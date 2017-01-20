## Instructions for providers of s/w components {#instructions-for-providers-of-s-w-components}

* [How to share your components](how-to-share-your-web-services-or-end-user-applications.md)
* [How to make your components interoperable](how-to-share-your-web-services-or-end-user-applications.md)
* [How to document your components](how-to-document-your-web-services-or-applications.md)









### ****Technical requirements**** {#technical-requirements}

In addition, if you want to be fully compliant with the OpenMinTeD interoperability requirements, please ensure that you adopt the following rules; if you fail to abide to them, it might still be possible to operate your s/w resources via the OpenMinTeD platform, but this cannot be guaranteed and interoperability with other resources will suffer loss.

*   Please, keep separate ancillary knowledge resources, e.g. models, annotation resources, etc. from the component itself; document and upload these also in the OpenMinTeD Registry following the procedure described in **_Guidelines for providers of ancillary knowledge resources_**. If you want to refer to these resources from the s/w metadata record, please use the resource identifier for the linking.
*   To ensure that provided s/w components can be scaled as required for different workloads, it is recommended that they are implemented in a stateless fashion, i.e. without the need to maintain information about one or more documents and the need to share this information with other instances of the same component. E.g. a component that counts all tokens in a corpus cannot be trivially scaled.
*   In addition to plain UIMA/uimaFIT and GATE-CREOLE descriptors, OpenMinTeD also supports Argo descriptors; further instructions for deploying UIMA components in Argo are found in Appendix E.

### ​Recommended ancillary knowledge resources {#recommended-ancillary-knowledge-resources}

In order to further encourage interoperability, OpenMinTeD makes specific recommendations about particular knowledge resources that TDM tools and services should use. These recommendations are in the areas of linguistics and of the initial domains of use targeted by OpenMinTeD. The current recommendations should not be seen as a final and static set. They will evolve with experience, and as OpenMinTeD is used for TDM of new domains. Users are therefore encouraged to use the existing recommendations, but to make use of others where these are not suitable.

TDM tools and services should use resources from the following initial list where possible. Where this is not possible, knowledge resource authors are encouraged to provide linkages between their own resource and those given here, or to any other widely used or standard Linked Data knowledge resource. This list of recommended resources should be seen as a first version, and will be extended.

*   Social sciences resources
    *   [TheSoz](http://www.gesis.org/en/services/research/thesauri-und-klassifikationen/social-science-thesaurus/)
*   Agriculture and agronomy resources
    *   [Agrovoc](http://aims.fao.org/agrovoc)
    *   Ontologies from [AgroPortal](http://agroportal.lirmm.fr/)
*   Life sciences resources
    *   [OboInOwl](http://purl.org/obo/owl/oboInOwl)
    *   MeSH ([available in LOD](http://hhs.github.io/meshrdf/))
    *   [BioC](http://bioc.sourceforge.net/)
    *   [NeuroLex](http://www.neurolex.org/)
    *   [BioLexicon](http://catalog.elra.info/product_info.php?products_id=1113)
*   Linguistic resources
    *   [LAPPS](http://vocab.lappsgrid.org/) (vocabulary of core linguistic objects)
    *   [Universal Dependencies](http://universaldependencies.org) (part of speech tags, features for morphology and syntactic dependencies)
    *   [OLIA](http://acoli.cs.uni-frankfurt.de/resources/olia/) (reference model and annotation models for morphology, morphosyntax, dependencies)
    *   [Penn Treebank](http://repository.upenn.edu/cgi/viewcontent.cgi?article=1603&context=cis_reports) (part of speech tags and features of morphology)
    *   [ISOcat](http://www.isocat.org/) / CCR (linguistic and metadata terminology)<sup><sup id="916464963798167-footnote-ref-39"><a href="#916464963798167-footnote-39">[39]</a></sup></sup>
    *   [GOLD](http://linguistics-ontology.org/version)(linguistic ontology)
*   Typesystems used by the s/w components integrated in the OpenMinTeD platform (GATE, DKPRO, ALVIS, ARGO and ILSP)

### ****Documentation/Metadata requirements**** {#documentation-metadata-requirements}

To be fully compatible with OpenMinTeD, you must

*   ensure that the s/w is distributed under a perpetual, world-wide, no-charge, royalty-free copyright/patent license that permits unrestricted use and allows unlimited redistribution
*   include in the metadata record a link to the licence document(s) with the terms and conditions under which it is provided, and attach the licence document(s) together with the resource
*   if you already have a PID for your resource (e.g. a URI or a HANDLE), make sure it is included in the metadata record
*   ensure that you version all your s/w resources and label the versions in an unambiguous way, preferably following the Semantic Versioning recommendations[^40].
*   ensure that you provide with your s/w resource appropriate machine-readable metadata embedded in the source code (where possible) and according to the relevant framework (e.g. uimaFIT Java annotations etc.); make sure that the metadata descriptors are properly identified an unambiguous way that makes them easy to distinguish and extract
*   for Java-based components, ensure that you use the Java fully qualified class naming conventions for naming your components; together with the Maven practices for registering packaging and version, this contributes to unique identifiers of the components
*   describe all the executional requirements for the proper operation of the s/w, i.e. required s/w libraries, ancillary resources, annotation schema dependencies etc.
*   describe the input and output requirements for your s/w, at least as regards the type of resource, the language (if required), data format and character encoding, and annotation types of the input/output resource
*   declare whether the s/w is downloadable or can only be accessed as a web service in the metadata.
*   ensure that you describe appropriately the functionalities of the s/w, both through the OMTD-SHARE component type vocabulary (pending link) as well as in a free text description, supplying more information for the user.

Further recommendations that contribute to interoperability include the following:

*   It is important that you provide the appropriate documentation for your resource (e.g. manuals, help files etc.), which you should also version along with the s/w and add as reference to your metadata record.
*   Recommend one of the publications about your resource as the one to be cited for scholarly attribution and add this information in the metadata record.
*   Make sure that you fill in the metadata record all the elements required for citing your resource<sup><sup id="916464963798167-footnote-ref-41"><a href="#916464963798167-footnote-41">[41]</a></sup></sup>, i.e. the creator of the resource, a title, the resource type and an identifier, and optionally, the publication date, the version and the publisher or distributor of
*   In all cases, where linking to other resources or entities (e.g. persons, projects etc.), please try to do this through unique and persistent identifiers of authority lists and sources, to the extent possible, documenting also the authority and/or scheme it adheres to.

[^37]: Details of GATE descriptors can be found at

[^38]: Mappings between the OMTD-SHARE and the Maven, UIMA/uimaFIT and CREOLE descriptors are included in _Section 5.2.2.3 – Recommended schema for s/w resources - Detailed presentation_

[^39]: ISOcat has redently moved to the

[^40]: 

[^41]: For citation, OpenMinTeD endorses the