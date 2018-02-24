### How to comply with OpenMinTeD interoperability specifications {#how-to-make-your-components-interoperable}

OpenMinTeD has defined a set of technical and legal specifications that intend to facilitate the secure and robust deployment of TDM applications running on scholarly content.
These specifications aim to support TDM experts by offering them a plethora of interoperable components that can interact seamlessly without complex manipulations; by selecting and combining appropriate components, they can build **end-to-end solutions** for the technology agnostic researchers; moreover, the specifications take into account the resources (content to be mined and ancillary knowledge resources) that interact with the applications and/or components. 

####Minimum requirements
{% blurb style='warning'%}
At present, the OpenMinTeD platform deploys

* **components** that support \(i.e. produce & consume\) **data in the [XML Metadata Interchange \(XMI\)](http://www.omg.org/spec/XMI/) format**, and more specifically the representation of a UIMA CAS; in the case of components that support other formats, appropriate readers and writers for converting XMI messages from and to the components’ format must also be provided[^1];
* **applications** that support as input file formats that are used for publications (e.g. PDF, PubMed XML, plain text etc.) or XMI (again as a UIMA CAS)[^2].
{% endblurb %}

As regards the **final output of the applications**, OpenMinTeD recommends the use of the XMI format for annotated corpora; other formats, such as the [WebAnnotation](https://www.w3.org/annotation/) standard, can also be used but _**only XMI-formatted annotated corpora** can be viewed with the OpenMinTeD annotation viewer and/or edited with the annotation editors_.[^3]

####Recommendations
If you want to be fully compliant with the OpenMinTeD interoperability requirements, please ensure that you adopt the following rules; if you fail to abide to them, it might still be possible to operate your software resources via the OpenMinTeD platform, but this cannot be guaranteed and interoperability with other resources will suffer loss.

To be fully compatible with OpenMinTeD, you must

* **Licensing**:
  * ensure that the software is distributed under a perpetual, world-wide, no-charge, royalty-free copyright/patent licence that permits unrestricted use and allows unlimited redistribution
  * include in the metadata record a link to the licence document\(s\) with the terms and conditions under which it is provided, and attach the licence document\(s\) together with 
the resource

{% blurb style='tip'%}
Please note that 
* FOSS licences are recommended for software resources
* You can use the [licence compatibility matrix](https://openminted.github.io/releases/license-matrix/) to check whether your components can be combined with other components on the basis of their licencing terms
{% endblurb %}
  
* **Operation and access**:
  * describe all the executional requirements for the proper operation of the software, i.e. required software libraries, ancillary knowledge resources, annotation schema dependencies, etc.
  * declare the mode of distribution/execution in the metadata (e.g. whether it's a web service)
  * describe the input and output requirements for your software, at least as regards the type of resource, the language \(if required\), data format, and annotation types of the input/output resource; 
* **Persistent and Unique identifiers**:
  * if you already have a PID for your resource \(e.g. a URI or a HANDLE\), make sure it is included in the metadata record \(cf. [resourceIdentifier](/components_resourceIdentifier.html) for more information\)
  * in the case of applications/components delivered 
    * via Maven, please provide the Maven coordinates in this element
    * as Docker images, provide the name for the application/component used in the image.
* **Versioning**: ensure that you version all your software resources and label the versions in an unambiguous way, preferably following the [Semantic Versioning recommendations](http://semver.org)
* **Formal description and documentation**:
  * ensure that you provide with your software appropriate machine-readable metadata embedded in the source code \(where possible\) and according to the relevant framework \(e.g. uimaFIT Java annotations etc.\); make sure that the metadata descriptors are properly identified in an unambiguous way that makes them easy to distinguish and extract
  * for Java-based components, ensure that you use the Java fully qualified class naming conventions for naming your components; together with the Maven practices for registering packaging and version, this contributes to unique identifiers of the components
  * in addition to plain UIMA/uimaFIT and GATE-CREOLE descriptors, OpenMinTeD also supports Argo descriptors
  * ensure that you describe appropriately the functionalities of the software, both through the OMTD-SHARE ontology class [function](/components_function.md) as well as in a free text description, supplying more information for the use
* **Scalability**: to ensure that provided software components can be scaled as required for different workloads, it is recommended that they are implemented in a stateless fashion, i.e. without the need to maintain information about one or more documents and the need to share this information with other instances of the same component
* **Re-usability of ancillary knowledge resources**: please, keep ancillary knowledge resources, e.g. models, annotation resources, etc., separate from the component itself; document and upload these also in the OpenMinTeD Registry following the procedure described in [_**Guidelines for providers of ancillary knowledge resources**_](/guidelines_for_providers_of_ancillary_resources/README.md). If you want to refer to these resources from the software metadata record, please add also the resource identifier in the relevant metadata element. You will find a list of recommended ancillary knowledge resources [here](/guidelines_for_providers_of_sw_resources/recommended-knowledge-resources.md); feel free to let us know of other resources that you think should be added to this list.

Further recommendations that contribute to interoperability include the following:

* **Documentation and citation**
  * It is important that you provide the appropriate documentation for your resource \(e.g. manuals, help files etc.\), which you should also version along with the software and add as reference to your metadata record. 
  * Recommend one of the publications about your resource as the one to be cited for scholarly attribution and add this information in the metadata record.
  * Make sure that you fill in the metadata record all the elements required for citing your resource[^4], i.e. the creator of the resource, a title, the resource type and an identifier, and optionally, the publication date, the version and the publisher or distributor.
* **Linking to other entities**: In all cases, where linking to other resources or entities \(e.g. persons, projects etc.\), please try to do this through unique and persistent identifiers of authority lists and sources, to the extent possible, documenting also the authority and/or scheme it adheres to.

---
[^1]: For applications built with the OpenMinTeD workflow editor, converters from PDF and other popular formats for publications into XMI are provided by OpenMinTeD. 
[^2]: For applications uploaded in OpenMinTeD that consume XMI, the appropriate converters for handling scholarly content input are provided by OpenMinTeD.
[^3]: For other types of output results (e.g. lists of named entities, lists of terms with statistical information etc.), application providers are welcome to use any format(s) they find fit.
[^4]: For citation, OpenMinTeD endorses the [Joint Declaration of Data Citation Principles](https://www.force11.org/group/joint-declaration-data-citation-principles-final), as well as the more specialised [RDA recommendations for data citation of evolving data](https://www.rd-alliance.org/system/files/RDA-DC-Recommendations_151020.pdf) and [DataCite guidelines](https://www.datacite.org/cite-your-data.html). 


