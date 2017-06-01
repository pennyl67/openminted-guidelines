## Sharing software components through OpenMinTeD {#instructions-for-providers-of-s-w-components}

The recommended way of providing _**software components**_ is through the Maven Central repository according to the following instructions:

* Please, put together in a single folder \(in the form that is required from the used technologies/frameworks\)
  * all files that implement the component \(e.g. Java classes etc.\)
  * licence text\(s\), preferably in a text file entitled "LICENCE.TXT" in order to be unambiguously recognised; in the case of multiple licences, they should be all aggregated in the same file
  * a readme notice, that describes the contents of the folder as well as any important notice for the compilation and execution of the component
  * all descriptors \(UIMA/uimaFIT, GATE CREOLE[^1], OMTD-SHARE etc.\) available for the component according to the implementation framework,
  * a Maven POM XML file, taking into account the recommendations described here.
* Pack them as a JAR using the respective Maven plugin.
* Upload them to the Maven repository according to the Maven guidelines.

You can then visit the OpenMinTeD registry at [https://services.openminted.eu](https://services.openminted.eu) where you can register your component in one of the following ways:

* edit from scratch the metadata using the OpenMinTeD editor
* upload an XML file with the OMTD-SHARE metadata record or
* submit the Maven coordinates; in this case,

  \(a\) if there is an OMTD-SHARE descriptor included in the package, it will be uploaded to the registry,  
  \(b\) otherwise, an OMTD-SHARE record can be partially converted from the Maven POM file and, potentially from elements included in the metadata descriptors supported by OpenMinTeD.

In all of these cases, the metadata record can be viewed and edited with the OpenMinTeD editor at the end of the process.

Further requirements and recommendations for achieving interoperability across components and with the content are presented [here](/guidelines_for_providers_of_sw_resources/how-to-make-your-components-interoperable.md).

[^1]: Details of GATE descriptors can be found at [https://gate.ac.uk/userguide/sec:creole-model:config](https://gate.ac.uk/userguide/sec:creole-model:config) although they do not currently contain many \(if any\) of the information needed to complete the OMTD-SHARE metadata descriptor. Note that this is changing to include more OpenMinTed like information much of which will be specified in a Maven POM rather than as CREOLE metadata. This is currently not documented as it relates to the next version of GATE that is still under active development.

