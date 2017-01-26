## Guide for deploying UIMA components in the Argo platform {#guide-for-deploying-uima-components-in-the-argo-platform}

Argo is able to use standard Java UIMA components, however they must be first packaged as UIMA PEAR (Processing Engine ARchive) files before they can be deployed within the Argo platform.

It is strongly recommended to use Maven, a build automation tool, to manage UIMA component projects, and a Maven pom.xml template (see further below) is available. The highlighted values within the pom.xml template are those expected to be configured by component developers.

The very minimum files required to produce a working UIMA component are:

1.  A standard UIMA XML descriptor (located under the desc folder at the root of the project).
2.  A Java class containing the implementation of the component (located under src/main/Java).
3.  A Maven pom.xml (adapted from the template).

Figure 1 shows the recommended layout of a very simple component project managed by Maven, using the example placeholder values found in the Maven pom.xml template. The UIMA XML descriptor should be named using the Maven artifactId value (e.g. uima-component) and reside under the desc directory and then a nested set of directories representing the Maven groupId value (e.g. xyz.company.uima).

Figure 1: Basic layout of a Maven-based UIMA component project

It is recommended to use the Maven artifactId and groupId to produce the UIMA Component ID (e.g the groupId xyz.company.uima and artifactId uima-component should result in a Component ID of xyz.company.uima.uima-component). The default configuration of the PEAR Packaging Maven plugin, within the pom.xml template, automates this procedure. A Component ID is intended to be unique and is not intended to be visible to Argo end-users.

Any Java dependencies of a UIMA component are expected to be included within a component’s PEAR file. The pom.xml template is configured to automatically package the Maven dependencies when building a PEAR file. However, to achieve Argo compatibility, **it is important to exclude the uimaj-core artifact and any artifacts representing UIMA Type Systems**. In the pom.xml template this is achieved by supplying the excludeArtifactIds configuration parameter of the the Maven Dependency plugin with a comma-delimited list of the affected artifactIds. Argo expects UIMA Type Systems to be installed separately and packaged as PEAR files, as for UIMA components.

A component may also contain an Argo XML descriptor file, although this is entirely optional. It is intended to provide additional metadata for a component. An Argo XML descriptor must:

*   Reside in the same directory as the component’s UIMA XML descriptor.
*   Have the same filename as the UIMA XML descriptor, but with a _.argo.xml_ suffix.

Figure 2 shows the location and name of an Argo XML descriptor file for a component with the ID of xyz.company.uima.uima-component, while Figure 3 shows the general format of the descriptor file itself.

Figure 2: Example file structure of a component containing Argo XML descriptor file

| &lt;argoDescriptor&gt; |
| --- |

Figure 3: Structure of an Argo XML descriptor

Within an Argo descriptor file, all of the sub-elements directly under the argoDescriptor element are optional.

The tags element can contain multiple tag elements, each containing a string value. These tag values are intended to be used within Argo’s component search facility, to assist end-users in finding relevant components.

The minimumMemoryinMbs element holds an integer value, setting the default value for the minimum of amount of memory (in Megabytes) required by this component when it is ran in a distributed workflow. This is important for determining the allocation of components to machines.

The interactive element contains a boolean value. This value is set to true when a component contains a custom web user interface, which requires interaction with the annotation model during a workflow execution. The only existing Argo component with this value set to true is the Manual Annotation Editor.

The configurationParametersMetaData can contain multiple configurationParameterMetaData elements, each one providing additional information about component configuration parameters found within the matching UIMA XML descriptor. A configurationParameterMetaDataelement must contain a name subelement (which has the same name as the configuration parameter it is referencing in the UIMA descriptor) and a uiType subelement (which is used by Argo to provide the most appropriate UI widget to the end-user). Valid values for uiType are _time_, _date_, _datetime_. _enum_, _password_, _type_, _document_ and _text_.

Figure 4 shows how configurationParameterMetaData elements are configured if their uiType value is either _time_, _date_ or _datetime_. The corresponding UIMA configuration parameter must be of type _string_. Argo needs to know how to format the time chosen by the end-user using a calendar UI widget, so this has to be specified in the format subelement, as demonstrated in Figure 4.

| &lt;configurationParameterMetaData&gt; |
| --- |

Figure 4: A date, time or datetime configuration parameter

For configuration parameters that have a fixed set of values, a uiType value of _enum_ is required. These fixed values should be listed as a set of value elements, nested within a values element, as shown in Figure 5.

| &lt;configurationParameterMetaData&gt; |
| --- |

Figure 5: An enum configuration parameter

Configuration parameters containing sensitive information, such as passwords, should use a uiType value of _password_. This hides the value of the parameter from the user and, once entered, does not get transmitted back to the Argo UI, for additional security. Additionally, it is also possible to specify the minimum and/or the maximum number of characters which this value can hold, using min and max elements within the valueConstraints element. See Figure 6 for an example.

| &lt;configurationParameterMetaData&gt; |
| --- |

Figure 6: A password configuration parameter

To make it easier for a user to select UIMA type(s) within the Argo UI, any configuration parameters representing types should have uiType value of _type_. This will result in a searchable list of all types, known to Argo, being displayed to the end-user when they are configuring the component, from which the required types can be selected.

| &lt;configurationParameterMetaData&gt; |
| --- |

Figure 8: A type configuration parameter

Configuration parameters which refer to local files and/or directories should have the uiType value of _document_. This will allow an end-user to select files from the Argo File Store using a file selector dialog. Figure 6 shows an example configuration and a table declaring the UI configuration parameters available to configure the file dialog can be found in Figure 7.

| &lt;configurationParameterMetaData&gt; |
| --- |

Figure 7: A document configuration parameter

| **selectFile** | Boolean | Allows a user to select a file in the dialog |
| --- | --- | --- |
| **selectFolder** | Boolean | Allows a user to select a folder in the dialog |
| **selectFilesRecursively** | Boolean | Recursively selects all of the files and/or folders, under the selected folders. |
| **hideFiles** | Boolean | Only show directories in the dialog |
| **windowCaption** | Boolean | A caption to display in the file browser window |

Figure 8: uiConfiguration elements

Configuration parameters that are likely to hold a large amount of text should use a uiType value of _text_. This will result in a larger text box being made available to the end-user. The size of the text area is configured using characterWidth and visibleLines elements, nested within the uiConfiguration element, as shown in Figure 9.

| &lt;configurationParameterMetaData&gt; |
| --- |

Figure 9: A text area configuration parameter

An example of a UIMA XML descriptor, along with its corresponding Argo XML descriptor, can be found further below.

**Maven pom.xml template for Argo components**

| &lt;project xmlns=&quot;http://maven.apache.org/POM/4.0.0&quot; xmlns:xsi=&quot;http://www.w3.org/2001/XMLSchema-instance&quot; xsi:schemaLocation=&quot;http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd&quot;&gt; |
| --- |

**Argo XML Descriptor example**

| &lt;argoDescriptor&gt; |
| --- |

**UIMA Analysis Engine XML Descriptor referenced by the Argo XML Descriptor**

| &lt;?xml version=&quot;1.0&quot; encoding=&quot;UTF-8&quot;?&gt; |
| --- |