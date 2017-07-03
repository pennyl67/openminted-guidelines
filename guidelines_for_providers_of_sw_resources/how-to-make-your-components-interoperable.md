### Achieving compatibility with OpenMinTeD and interoperability across TDM resources {#how-to-make-your-components-interoperable}

If you want to be fully compliant with the OpenMinTeD interoperability requirements, please ensure that you adopt the following rules; if you fail to abide to them, it might still be possible to operate your software resources via the OpenMinTeD platform, but this cannot be guaranteed and interoperability with other resources will suffer loss.

To be fully compatible with OpenMinTeD, you must

* **Licensing**:
  * ensure that the software is distributed under a perpetual, world-wide, no-charge, royalty-free copyright/patent licence that permits unrestricted use and allows unlimited redistribution
  * include in the metadata record a link to the licence document\(s\) with the terms and conditions under which it is provided, and attach the licence document\(s\) together with the resource; FOSS licences are recommended for software resources
* **Persistent and Unique identifiers**:
  * if you already have a PID for your resource \(e.g. a URI or a HANDLE\), make sure it is included in the metadata record \(cf. [identifier](/publications_identifier.md) for more information\)
  * in the case of components delivered via Maven, please provide the Maven identifier in the record
* **Versioning**: ensure that you version all your software resources and label the versions in an unambiguous way, preferably following the [Semantic Versioning recommendations](http://semver.org)
* **Formal description and documentation**:
  * ensure that you provide with your software resource appropriate machine-readable metadata embedded in the source code \(where possible\) and according to the relevant framework \(e.g. uimaFIT Java annotations etc.\); make sure that the metadata descriptors are properly identified in an unambiguous way that makes them easy to distinguish and extract
  * for Java-based components, ensure that you use the Java fully qualified class naming conventions for naming your components; together with the Maven practices for registering packaging and version, this contributes to unique identifiers of the components
  * In addition to plain UIMA/uimaFIT and GATE-CREOLE descriptors, OpenMinTeD also supports Argo descriptors; further instructions for deploying UIMA components in Argo are found [here](/guidelines_for_providers_of_sw_resources/guide_for_deploying_uima_components_in_.md)
  * ensure that you describe appropriately the functionalities of the software, both through the OMTD-SHARE [component type ](/components_componentType.md) or [applicationFunction](/components_applicationFunction.md) vocabulary as well as in a free text description, supplying more information for the use
* **Operation and access**:
  * declare whether the software is downloadable or can only be accessed as a web service in the metadata
  * describe all the executional requirements for the proper operation of the software, i.e. required software libraries, ancillary resources, annotation schema dependencies, etc.
  * describe the input and output requirements for your software, at least as regards the type of resource, the language \(if required\), data format and character encoding, and annotation types of the input/output resource; 
  * support at least the following data formats, given that OpenMinTeD has endorsed the use of 
    * the [XML Metadata Interchange](http://www.omg.org/spec/XMI/) \(XMI\) format, specifically the representation of a [UIMA CAS](https://uima.apache.org/d/uimaj-2.9.0/references.html#ugr.ref.xmi) to encode annotations on text in particular when exchanging data between components within a [workflow](https://guidelines.openminted.eu/GLOSSARY.html#workflow) and
    * the [WebAnnotation](https://www.w3.org/annotation/) standard to make annotations produced by OpenMinTeD workflows accessible to third parties and to encode annotations above the text level, e.g. on [document](https://guidelines.openminted.eu/GLOSSARY.html#document)/collection level.
* **Scalability**: To ensure that provided software components can be scaled as required for different workloads, it is recommended that they are implemented in a stateless fashion, i.e. without the need to maintain information about one or more documents and the need to share this information with other instances of the same component. E.g. a component that counts all tokens in a corpus cannot be trivially scaled.
* **Re-usability of ancillary resources**:
  * Please, keep ancillary knowledge resources, e.g. models, annotation resources, etc., separate from the component itself; document and upload these also in the OpenMinTeD Registry following the procedure described in [_**Guidelines for providers of ancillary knowledge resources**_](/guidelines_for_providers_of_ancillary_resources/README.md). If you want to refer to these resources from the software metadata record, please use the resource identifier for the linking.



Further recommendations that contribute to interoperability include the following:

* **Documentation and citation**
  * It is important that you provide the appropriate documentation for your resource \(e.g. manuals, help files etc.\), which you should also version along with the software and add as reference to your metadata record. 
  * Recommend one of the publications about your resource as the one to be cited for scholarly attribution and add this information in the metadata record.
  * Make sure that you fill in the metadata record all the elements required for citing your resource[^1], i.e. the creator of the resource, a title, the resource type and an identifier, and optionally, the publication date, the version and the publisher or distributor.
* **Linking to other entities**: In all cases, where linking to other resources or entities \(e.g. persons, projects etc.\), please try to do this through unique and persistent identifiers of authority lists and sources, to the extent possible, documenting also the authority and/or scheme it adheres to.

---

[^1]: For citation, OpenMinTeD endorses the [Joint Declaration of Data Citation Principles](https://www.force11.org/group/joint-declaration-data-citation-principles-final), as well as the more specialised [RDA recommendations for data citation of evolving data](https://www.rd-alliance.org/system/files/RDA-DC-Recommendations_151020.pdf) and [DataCite guidelines](https://www.datacite.org/cite-your-data.html).

