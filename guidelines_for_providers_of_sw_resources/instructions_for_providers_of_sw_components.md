## Sharing software through OpenMinTeD {#instructions-for-providers-of-s-w-components}

OpenMinTeD acts as a facilitator for TDM processing operations rather than as a repository of content and software resources. 

For software, it relies on specific repositories through which the software is made publicly available; at the time of execution, it is retrieved from these repositories in order to be deployed within the OpenMinTeD infrastructure. 



Furthermore, to overcome hurdles associated with platform dependent implementations, OpenMinTeD has decided to use Docker images for software components. For components compatible with specific frameworks, dockerization is undertaken by OpenMinTeD. 

Alternatively, TDM component developers can also expose their software through the Processing Web Service API layer that has been specified by OpenMinTeD.



There are, therefore, three ways you can provide TDM software in OpenMinTeD:

components compatible with UIMA or GATE frameworks can be uploaded in the Maven Central repository and registered by declaring the respective Maven coordinates which uniquely specify their  location; dockerization for these components is undertaken by OpenMinTeD;

components created with other technologies or other TDM-related frameworks must be packaged  and registered directly as Docker images;

web services which are installed and maintained outside the OpenMinTeD platform are accessed via an appropriate client which is also packaged in a Docker image; they must be registered in OpenMinTeD with the URL that specifies their location.







The recommended way of providing _**software components**_ is through the [Maven](http://maven.apache.org/) Central repository according to the following instructions:

* Please, put together in a single folder \(in the form that is required from the used technologies/frameworks\)
  * all files that implement the component \(e.g. Java classes etc.\)
  * licence text\(s\), preferably in a text file entitled "LICENCE.TXT" in order to be unambiguously recognised; in the case of multiple licences, they should be all aggregated in the same file
  * a readme notice, that describes the contents of the folder as well as any important notice for the compilation and execution of the component
  * all descriptors \(UIMA/uimaFIT, GATE CREOLE, OMTD-SHARE etc.\) available for the component according to the implementation framework,
  * a Maven POM XML file.
* Pack them as a JAR using the respective Maven plugin.
* Upload them to the Maven repository according to the Maven guidelines.

You can then visit the OpenMinTeD registry at [https://services.openminted.eu](https://services.openminted.eu) where you can register your component in one of the following ways:

* edit from scratch the metadata using the OpenMinTeD editor
* upload an XML file with the OMTD-SHARE metadata record with the Maven coordinates filled in the relevant metadata element, or
* submit the Maven coordinates; in this case,

  \(a\) if there is an OMTD-SHARE descriptor included in the package, it will be uploaded to the registry,  
  \(b\) otherwise, an OMTD-SHARE record can be partially converted from the Maven POM file and, potentially from elements included in the metadata descriptors supported by OpenMinTeD.

In all of these cases, the metadata record can be viewed and edited with the OpenMinTeD editor at the end of the process.

Further requirements and recommendations for achieving interoperability across components and with the content are presented [here](/guidelines_for_providers_of_sw_resources/how-to-make-your-components-interoperable.md).

