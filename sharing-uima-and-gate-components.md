### Sharing UIMA and GATE components

**Step 1**

You can provide components compatible with the UIMA and GATE frameworks through the Maven Central repository \([https://mvnrepository.com/\](https://mvnrepository.com/\)\) according to the following instructions:

* Please, put together in a single folder \(in the form that is required from the used technologies/frameworks\)
  * all files that implement the component \(e.g. Java classes etc.\)
  * licence text\(s\), preferably in a text file entitled "LICENCE.TXT" in order to be unambiguously recognised; in the case of multiple licences, they should be all aggregated in the same file
  * a readme notice, that describes the contents of the folder as well as any important notice for the compilation and execution of the component
  * all descriptors \(UIMA/uimaFIT, GATE CREOLE, OMTD-SHARE etc.\) available for the component according to the implementation framework; OMTD-SHARE descriptors are identified with the filename extension ".omtds.xml"
  * a descriptors.txt file in the folder META-INF/eu.openminted/share with a list of the descriptors
  * a Maven POM XML file.
* Pack them as a JAR using the respective Maven plugin.
* Upload them to the Central Maven repository according to the Maven guidelines \([http://maven.apache.org/guides/mini/guide-central-repository-upload.html\](http://maven.apache.org/guides/mini/guide-central-repository-upload.html\)\).



**Step 2**

You can then visit the OpenMinTeD registry where you can register your component in one of the following ways:

* create from scratch the [OMTD-SHARE metadata](/guidelines_for_providers_of_sw_resources/recommended_schema_for_sw_resources.md) record \(minimal schema\) using the OpenMinTeD editor; in this case, you must provide the Maven coordinates through the element _&lt;distributionLocation&gt;_, e.g. `<distributionLocation>mvn:de.tudarmstadt.ukp.dkpro.core:de.tudarmstadt.ukp.dkpro.core.berkeleyparser-gpl:1.9.0-SNAPSHOT#de.tudarmstadt.ukp.dkpro.core.berkeleyparser.BerkeleyParser</distributionLocation>`
* upload the [OMTD-SHARE metadata record](/guidelines_for_providers_of_sw_resources/recommended_schema_for_sw_resources.md) as an XML file with the Maven coordinates filled in the metadata element &lt;distributionLocation&gt; as in the above example, or
* submit the Maven coordinates directly in the interface; in this case,
  * if the package includes one or more  OMTD-SHARE files corresponding to the components contained in the package, the available components will be displayed to the user, the user will select the component to register, the metadata will be validated and, if valid, uploaded to the registry;
  * if there are no OMTD-SHARE files in the package, an OMTD-SHARE record can be partially converted from the Maven POM file and the user will be prompted to fill in the missing information.

In all of these cases, the metadata record can be viewed and edited at the end of the process.

Components provided in this mode are dockerized by OpenMinTeD.

Further requirements and recommendations for achieving interoperability across components and with the content resources are presented here.

