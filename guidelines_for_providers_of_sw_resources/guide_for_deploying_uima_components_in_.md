## Guide for deploying UIMA components in the Argo platform {#guide-for-deploying-uima-components-in-the-argo-platform}

Argo is able to use standard Java UIMA components, however they must be first packaged as UIMA PEAR (Processing Engine ARchive) files before they can be deployed within the Argo platform.

It is strongly recommended to use Maven, a build automation tool, to manage UIMA component projects, and a Maven pom.xml template (see further below) is available. The highlighted values within the pom.xml template are those expected to be configured by component developers.

The very minimum files required to produce a working UIMA component are:

1.  A standard UIMA XML descriptor (located under the desc folder at the root of the project).
2.  A Java class containing the implementation of the component (located under src/main/Java).
3.  A Maven pom.xml (adapted from the template).

Figure 1 shows the recommended layout of a very simple component project managed by Maven, using the example placeholder values found in the Maven pom.xml template. The UIMA XML descriptor should be named using the Maven artifactId value (e.g. uima-component) and reside under the desc directory and then a nested set of directories representing the Maven groupId value (e.g. xyz.company.uima).

![](/assets/Figure1.jpg)

Figure 1: Basic layout of a Maven-based UIMA component project

It is recommended to use the Maven artifactId and groupId to produce the UIMA Component ID (e.g the groupId xyz.company.uima and artifactId uima-component should result in a Component ID of xyz.company.uima.uima-component). The default configuration of the PEAR Packaging Maven plugin, within the pom.xml template, automates this procedure. A Component ID is intended to be unique and is not intended to be visible to Argo end-users.

Any Java dependencies of a UIMA component are expected to be included within a component’s PEAR file. The pom.xml template is configured to automatically package the Maven dependencies when building a PEAR file. However, to achieve Argo compatibility, **it is important to exclude the uimaj-core artifact and any artifacts representing UIMA Type Systems**. In the pom.xml template this is achieved by supplying the excludeArtifactIds configuration parameter of the the Maven Dependency plugin with a comma-delimited list of the affected artifactIds. Argo expects UIMA Type Systems to be installed separately and packaged as PEAR files, as for UIMA components.

A component may also contain an Argo XML descriptor file, although this is entirely optional. It is intended to provide additional metadata for a component. An Argo XML descriptor must:

*   Reside in the same directory as the component’s UIMA XML descriptor.
*   Have the same filename as the UIMA XML descriptor, but with a _.argo.xml_ suffix.

Figure 2 shows the location and name of an Argo XML descriptor file for a component with the ID of xyz.company.uima.uima-component, while Figure 3 shows the general format of the descriptor file itself.

![](/assets/Figure2.jpg)

Figure 2: Example file structure of a component containing Argo XML descriptor file


```
<argoDescriptor>
<tags>
		<tag>{string}/tag>
		...
	</tags>
<minimumMemoryInMbs>{integer}</minimumMemoryInMbs>
	<interactive>[true/false]</interactive>
	<configurationParametersMetaData>
		<configurationParameterMetaData>...</configurationParameterMetaData>
		...
	<configurationParametersMetaData>
</argoDescriptor>

```
Figure 3: Structure of an Argo XML descriptor

Within an Argo descriptor file, all of the sub-elements directly under the argoDescriptor element are optional.

The tags element can contain multiple tag elements, each containing a string value. These tag values are intended to be used within Argo’s component search facility, to assist end-users in finding relevant components.

The minimumMemoryinMbs element holds an integer value, setting the default value for the minimum of amount of memory (in Megabytes) required by this component when it is ran in a distributed workflow. This is important for determining the allocation of components to machines.

The interactive element contains a boolean value. This value is set to true when a component contains a custom web user interface, which requires interaction with the annotation model during a workflow execution. The only existing Argo component with this value set to true is the Manual Annotation Editor.

The configurationParametersMetaData can contain multiple configurationParameterMetaData elements, each one providing additional information about component configuration parameters found within the matching UIMA XML descriptor. A configurationParameterMetaDataelement must contain a name subelement (which has the same name as the configuration parameter it is referencing in the UIMA descriptor) and a uiType subelement (which is used by Argo to provide the most appropriate UI widget to the end-user). Valid values for uiType are _time_, _date_, _datetime_. _enum_, _password_, _type_, _document_ and _text_.

Figure 4 shows how configurationParameterMetaData elements are configured if their uiType value is either _time_, _date_ or _datetime_. The corresponding UIMA configuration parameter must be of type _string_. Argo needs to know how to format the time chosen by the end-user using a calendar UI widget, so this has to be specified in the format subelement, as demonstrated in Figure 4.



```
<configurationParameterMetaData>
	<name>timeParam</name>
	<uiType>time</uiType>
	<uiConfiguration>
		<format>HH:mm:ss</format>
	</uiConfiguration>
</configurationParameterMetaData>

```
Figure 4: A date, time or datetime configuration parameter

For configuration parameters that have a fixed set of values, a uiType value of _enum_ is required. These fixed values should be listed as a set of value elements, nested within a values element, as shown in Figure 5.



```
<configurationParameterMetaData>
	<name>enumParam</name>
	<uiType>enum</uiType>
	<values>
		<value>red</value>
		<value>green</value>
		<value>blue</value>
	</values>
</configurationParameterMetaData>

```

Figure 5: An enum configuration parameter

Configuration parameters containing sensitive information, such as passwords, should use a uiType value of _password_. This hides the value of the parameter from the user and, once entered, does not get transmitted back to the Argo UI, for additional security. Additionally, it is also possible to specify the minimum and/or the maximum number of characters which this value can hold, using min and max elements within the valueConstraints element. See Figure 6 for an example.



```
<configurationParameterMetaData>
	<name>passwordParam</name>
	<uiType>password</uiType>
	<valueConstraints>
		<min>5</min>
		<max>10</max>
	</valueConstraints>
</configurationParameterMetaData>

```

Figure 6: A password configuration parameter

To make it easier for a user to select UIMA type(s) within the Argo UI, any configuration parameters representing types should have uiType value of _type_. This will result in a searchable list of all types, known to Argo, being displayed to the end-user when they are configuring the component, from which the required types can be selected. See Figure 7 for an example.


```
<configurationParameterMetaData>
	<name>typeParam</name>
	<uiType>type</uiType>
</configurationParameterMetaData>

```

Figure 7: A type configuration parameter

Configuration parameters which refer to local files and/or directories should have the uiType value of _document_. This will allow an end-user to select files from the Argo File Store using a file selector dialog. Figure 8 shows an example configuration and a table declaring the UI configuration parameters available to configure the file dialog can be found in Figure 9.



```
<configurationParameterMetaData>
	<name>documentParam</name>
	<uiType>document</uiType>
	<uiConfiguration>
		<selectFile>true</selectFile>
		<selectFolder>false</selectFolder>
		<selectFilesRecursively>false</selectFilesRecursively>
		<hideFiles>false</hideFiles>
		<windowCaption>Save file as...</windowCaption>
	</uiConfiguration>
</configurationParameterMetaData>

```

Figure 8: A document configuration parameter

| **selectFile** | Boolean | Allows a user to select a file in the dialog |
| --- | --- | --- |
| **selectFolder** | Boolean | Allows a user to select a folder in the dialog |
| **selectFilesRecursively** | Boolean | Recursively selects all of the files and/or folders, under the selected folders. |
| **hideFiles** | Boolean | Only show directories in the dialog |
| **windowCaption** | Boolean | A caption to display in the file browser window |

Figure 9: uiConfiguration elements

Configuration parameters that are likely to hold a large amount of text should use a uiType value of _text_. This will result in a larger text box being made available to the end-user. The size of the text area is configured using characterWidth and visibleLines elements, nested within the uiConfiguration element, as shown in Figure 10.



```
<configurationParameterMetaData>
	<name>textAreaParam</name>
	<uiType>text</uiType>
	<uiConfiguration>
		<characterWidth>30</characterWidth>
		<visibleLines>5</visibleLines>
	</uiConfiguration>
</configurationParameterMetaData>

```
Figure 10: A text area configuration parameter

An example of a UIMA XML descriptor, along with its corresponding Argo XML descriptor, can be found further below.

**Maven pom.xml template for Argo components**

```
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
 <modelVersion>4.0.0</modelVersion>
 <groupId>xyz.company.uima</groupId>
 <artifactId>uima-component</artifactId>
 <version>1.0</version>

 <build>
 <resources>
 <resource>
 <directory>desc</directory>
 </resource>
 <resource>
 <directory>src/main/resources</directory>
 </resource>
 </resources>
 <plugins>
<plugin>
 <groupId>org.apache.maven.plugins</groupId>
 <artifactId>maven-dependency-plugin</artifactId>
 <version>2.4</version>
 <executions>
 <execution>
 <id>copy-dependencies</id>
 <phase>prepare-package</phase>
 <goals>
 <goal>copy-dependencies</goal>
 </goals>
 <configuration>
 <stripVersion>true</stripVersion> <outputDirectory>${project.build.directory}/pearPackaging/lib</outputDirectory>
 <overWriteReleases>true</overWriteReleases>
 <overWriteSnapshots>true</overWriteSnapshots>
 <includeScope>runtime</includeScope>
 				<excludeArtifactIds>U_compareTypeSystem,uimaj-core</excludeArtifactIds>
 </configuration>
 </execution>
 </executions>
 </plugin>
 <plugin>
 <groupId>org.apache.uima</groupId>
 <artifactId>PearPackagingMavenPlugin</artifactId>
 <version>2.4.0</version>
 <extensions>true</extensions>
 <executions>
 <execution>
 <phase>package</phase>
 <configuration> <mainComponentDesc>desc/xyz/company/uima/uima-component.xml</mainComponentDesc> <componentId>${project.groupId}.${project.artifactId}</componentId>
 </configuration>
 <goals>
 <goal>package</goal>
 </goals>
 </execution>
 </executions>
 </plugin>
 <plugin>
 <groupId>org.apache.maven.plugins</groupId>
 <artifactId>maven-install-plugin</artifactId>
 <version>2.3.1</version>
 <executions>
 <execution>
 <phase>install</phase>
 <configuration>
 <packaging>pear</packaging>
 <groupId>${project.groupId}</groupId>
 <artifactId>${project.artifactId}</artifactId>
 <version>${project.version}</version>
 <file> ${project.build.directory}/${project.groupId}.${project.artifactId}.pear
 </file>
 </configuration>
 <goals>
 <goal>install-file</goal>
 </goals>
 </execution>
 </executions>
 </plugin>
 </plugins>

 <pluginManagement>
 <plugins>
 <plugin>
 <groupId>org.eclipse.m2e</groupId>
 <artifactId>lifecycle-mapping</artifactId>
 <version>1.0.0</version>
 <configuration>
 <lifecycleMappingMetadata>
 <pluginExecutions> 
 <pluginExecution>
 <pluginExecutionFilter>
 <groupId>org.apache.maven.plugins</groupId>
 <artifactId>maven-dependency-plugin</artifactId>
 <versionRange>[1.0.0,)</versionRange>
 <goals>
 <goal>copy-dependencies</goal>
 </goals>
 </pluginExecutionFilter>
 <action>
 <execute>
 <runOnIncremental>false</runOnIncremental>
 </execute>
 </action>
 </pluginExecution>
 </pluginExecutions>
 </lifecycleMappingMetadata>
 </configuration>
 </plugin>
 </plugins>
 </pluginManagement>
 </build>

 
 
 <dependencies>
 <dependency>
 <groupId>org.apache.uima</groupId>
 <artifactId>uimaj-core</artifactId>
 <version>2.7.0</version>
 </dependency>
 <dependency>
 <groupId>org.u_compare</groupId>
 <artifactId>U_compareTypeSystem</artifactId>
 <version>1.1</version>
 </dependency>
 </dependencies>
</project>

```


**Argo XML Descriptor example**

```
<argoDescriptor>
<tags>
		<tag>categoryA</tag>
		<tag>finance</tag>
	</tags>
<minimumMemoryInMbs>256</minimumMemoryInMbs>
	<interactive>false</interactive>
	<configurationParametersMetaData>
		<configurationParameterMetaData>
			<name>timeParam</name>
			<uiType>time</uiType>
			<uiConfiguration>
				<format>HH:mm:ss</format>
			</uiConfiguration>
		</configurationParameterMetaData>
		<configurationParameterMetaData>
			<name>dateParam</name>
			<uiType>date</uiType>
			<uiConfiguration>
				<format>yyyy/MM/dd</format>
			</uiConfiguration>
		</configurationParameterMetaData>
		<configurationParameterMetaData>
			<name>dateTimeParam</name>
			<uiType>datetime</uiType>
			<uiConfiguration>
				<format>yyyy/MM/dd HH:mm:ss</format>
			</uiConfiguration>
		</configurationParameterMetaData>	
		<configurationParameterMetaData>
			<name>enumParam</name>
			<uiType>enum</uiType>
			<values>
				<value>red</value>
				<value>green</value>
				<value>blue</value>
			</values>
		</configurationParameterMetaData>
		<configurationParameterMetaData>
			<name>passwordParam</name>
			<uiType>password</uiType>
			<uiConfiguration>
			</uiConfiguration>
			<valueConstraints>
				<min>5</min>
				<max>10</max>
			</valueConstraints>
		</configurationParameterMetaData>
		<configurationParameterMetaData>
			<name>typeParam</name>
			<uiType>type</uiType>
			<uiConfiguration>
			</uiConfiguration>
		</configurationParameterMetaData>
		<configurationParameterMetaData>
			<name>documentParam</name>
			<uiType>document</uiType>
			<uiConfiguration>
				<selectFile>true</selectFile>
				<selectFolder>false</selectFolder>
				<selectFilesRecursively>false</selectFilesRecursively>
				<hideFiles>false</hideFiles>
				<windowCaption>Save file as...</windowCaption>
			</uiConfiguration>
		</configurationParameterMetaData>
		<configurationParameterMetaData>
			<name>textAreaParam</name>
			<uiType>text</uiType>
			<uiConfiguration>
				<characterWidth>30</characterWidth>
				<visibleLines>5</visibleLines>
			</uiConfiguration>
		</configurationParameterMetaData>
	</configurationParametersMetaData>
</argoDescriptor>

```


**UIMA Analysis Engine XML Descriptor referenced by the Argo XML Descriptor**

```
<?xml version="1.0" encoding="UTF-8"?>
<analysisEngineDescription xmlns="http://uima.apache.org/resourceSpecifier">
<frameworkImplementation>org.apache.uima.Java</frameworkImplementation>
 	<primitive>true</primitive>
<annotatorImplementationName>xyz.company.uima.UimaComponent</annotatorImplementationName>
 	<analysisEngineMetaData>
 		<name>UIMA Component</name>
 		<description/>
 		<version>1.0</version>
 		<vendor/>
 		<configurationParameters>
 			<configurationParameter>
 			<name>timeParam</name>
 			<type>String</type>
 			<multiValued>false</multiValued>
 			<mandatory>false</mandatory>
 			</configurationParameter>
 			<configurationParameter>
 			<name>dateParam</name>
 			<type>String</type>
 			<multiValued>false</multiValued>
 			<mandatory>false</mandatory>
 			</configurationParameter>
 			<configurationParameter>
 <name>dateTimeParam</name>
 <type>String</type>
 <multiValued>false</multiValued>
 <mandatory>false</mandatory>
</configurationParameter>
 		<configurationParameter>
 		<name>enumParam</name>
 		<type>String</type>
 		<multiValued>false</multiValued>
 		<mandatory>false</mandatory>
 		</configurationParameter>
<configurationParameter>
 <name>passwordParam</name>
 <type>String</type>
 <multiValued>false</multiValued>
 <mandatory>false</mandatory>
</configurationParameter>
<configurationParameter>
 <name>typeParam</name>
 <type>String</type>
 <multiValued>false</multiValued>
 <mandatory>false</mandatory>
</configurationParameter>
<configurationParameter>
 <name>documentParam</name>
 <type>String</type>
 <multiValued>false</multiValued>
 <mandatory>false</mandatory>
</configurationParameter>
<configurationParameter>
 <name>textAreaParam</name>
 <type>String</type>
 <multiValued>false</multiValued>
 <mandatory>false</mandatory>
</configurationParameter>
</configurationParameters>
<configurationParameterSettings/>
<typeSystemDescription/>
 		<typePriorities/>
 		<fsIndexCollection/>
 		<capabilities>
 		<capability>
 		<inputs/>
 		<outputs/>
 		<languagesSupported/>
 		</capability>
 	</capabilities>
 	<operationalProperties>
 		<modifiesCas>true</modifiesCas>
 		<multipleDeploymentAllowed>true</multipleDeploymentAllowed>
 		<outputsNewCASes>false</outputsNewCASes>
 		</operationalProperties>
 	</analysisEngineMetaData>
 	<resourceManagerConfiguration/>
</analysisEngineDescription>

```



