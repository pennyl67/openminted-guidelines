### How to register your components {#how-to-share-your-components}

The recommended way of providing **_software components_ **is through the Maven Central repository according to the following instructions:

*   Please, put together in a single folder (in the form that is required from the used technologies/frameworks)
    *   all files that implement the component (e.g. Java classes etc.)
    *   licence text(s), preferably named as &quot;LICENCE.TXT&quot; in order to be unambiguously recognised; in the case of multiple licences, they should be all aggregated in the same file
    *   a readme notice, that describes the contents of the folder as well as any important notice for the compilation and execution of the component
    *   all descriptors (UIMA/uimaFIT, GATE CREOLE[^1], OMTD-SHARE etc.) available for the component according to the implementation framework,
    *   a Maven POM XML file.
*   Pack them as a JAR using the respective Maven plugin.
*   Upload them to the Maven repository according to the Maven guidelines
*   Finally, submit the Maven coordinates in the OMTD registry; in this case, the metadata record will be partially converted from the Maven POM file and, potentially from elements included in the metadata descriptors supported by OpenMinTeD (UIMA/uimaFIT, CREOLE, and then you can enrich it using the OpenMinTeD editor.

[^1] Details of GATE descriptors can be found at [https://gate.ac.uk/userguide/sec:creole-model:config](https://gate.ac.uk/userguide/sec:creole-model:config) although they do not currently contain many (if any) of the information needed to complete the OMTD-SHARE metadata descriptor. Note that this is changing to include more OpenMinTed like information much of which will be specified in a Maven POM rather than as CREOLE metadata. This is currently not documented as it relates to the next version of GATE that is still under active development.