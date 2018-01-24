### Sharing UIMA and GATE components through MAVEN

You can provide components compatible with the [UIMA](https://uima.apache.org/) and [GATE](https://gate.ac.uk/) frameworks through the [Maven Central repository](https://mvnrepository.com/) according to the following instructions.

#### **Step 1 - Preparing and packaging**

* Please, put together in a single folder \(in the form that is required from the used technologies/frameworks\)
  * all files that implement the component \(e.g. Java classes etc.\)
  * licence text\(s\), preferably in a text file entitled "LICENCE.TXT" in order to be unambiguously recognised; in the case of multiple licences, they should be all aggregated in the same file
  * a "readme" notice, that describes the contents of the folder as well as any important notice for the compilation and execution of the component
  * all descriptors \(UIMA/uimaFIT, GATE CREOLE, OMTD-SHARE etc.\) available for the component according to the implementation framework; OMTD-SHARE descriptors must be identified with the filename extension ".omtds.xml"[^1]
  * a "DESCRIPTORS.TXT" file in the folder META-INF/eu.openminted.share with a list of the descriptors
  * a Maven POM XML file.
* Pack them as a JAR using the respective Maven plugin.
* Upload them to the Maven repository according to the Maven guidelines \([http://maven.apache.org/guides/mini/guide-central-repository-upload.html](http://maven.apache.org/guides/mini/guide-central-repository-upload.html)).

#### **Step 2 - Registering in OpenMinTeD**

You can then visit the [OpenMinTeD registry](https://services.openminted.eu/resourceRegistration/component) where you can register your component in one of the following ways:

* create from scratch the OMTD-SHARE metadata record \(minimal schema\) using the OpenMinTeD editor; in this case, you must provide the Maven coordinates through the element _&lt;distributionLocation&gt;_, e.g. `<distributionLocation>mvn:de.tudarmstadt.ukp.dkpro.core:de.tudarmstadt.ukp.dkpro.core.berkeleyparser-gpl:1.9.0-SNAPSHOT#de.tudarmstadt.ukp.dkpro.core.berkeleyparser.BerkeleyParser</distributionLocation>`
* upload the OMTD-SHARE metadata record[^2] as an XML file with the Maven coordinates filled in the relevant metadata element as in the above example, or
* submit the Maven coordinates directly in the interface; in this case, 
  * if the package includes one or more  OMTD-SHARE files corresponding to the components contained in the package, the available components will be displayed to the user, the user will select the component to register, the metadata will be validated and, if valid, uploaded to the registry; 
  * if there are no OMTD-SHARE files in the package, an OMTD-SHARE record can be partially converted from the Maven POM file and other descriptors and the user will be prompted to fill in the missing information.

In all of these cases, the metadata record can be viewed and edited at the end of the process.

Components provided in this mode are dockerized by OpenMinTeD.

Further requirements and recommendations for achieving interoperability across components and with the content resources are presented [here](/guidelines_for_providers_of_sw_resources/how-to-make-your-components-interoperable.md).

[^1]: You will find more information on how to embed the OMTD-SHARE metadata records in the package and how to use related tooling at https://builds.openminted.eu/view/WP%205.2/job/OpenMinTeD%20SHARE%20Annotations/eu.openminted.share.annotations%24omtd-share-annotations-doc/doclinks/1/#sect_introduction.
[^2]: You can find example metadata records [here](https://openminted.github.io/releases/omtd-share/3.0.2/).

