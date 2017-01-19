### ​Documentation/Metadata requirements {#documentation-metadata-requirements}

To be fully compatible with OpenMinTeD, you must

*   ensure that the resource is distributed under Open Access conditions
*   include in the metadata record a link to the licence document that describes the terms and conditions under which it is provided, and attach the licence document together with the resource
*   if you already have a PID for your resource (e.g. a URI or a HANDLE), make sure it is included in the metadata record.
*   provide linkage between your resource and other resources (domain-specific or generic resources); for links between knowledge resources in the Linked Data paradigm, mapping should be expressed through RDF statements, using relations from [SKOS](https://www.w3.org/2004/02/skos/), together with the following OWL and RDF object properties: owl:sameAs, owl:equivalentClass, owl:equivalentProperty, rdfs:subClassOf, rdfs:subPropertyOf.
*   version all your resources and label the versions in an unambiguous way, preferably following the [Semantic Versioning recommendations](/semver.org)[^30].

The following recommendations contribute to interoperability but are not yet enforced:

*   It is important that you provide the appropriate documentation for your resource (e.g. publications about the design and construction of the corpus etc.), which you should also version along with the knowledge resource and add as reference to your metadata record.
*   Recommend one of the publications about your resource as the one to be cited for scholarly attribution and add this information in the metadata record.
*   Make sure that you fill in the metadata record all the elements required for citing your resource, i.e. the creator of the resource, a title, the resource type and an identifier, and optionally, the publication date, the version and the publisher or distributor of
*   Use standard classification vocabularies (e.g. MeSH<sup><sup id="916464963798167-footnote-ref-32"><a href="#916464963798167-footnote-32">[32]</a></sup></sup>, DDC<sup><sup id="916464963798167-footnote-ref-33"><a href="#916464963798167-footnote-33">[33]</a></sup></sup>, LCSH<sup><sup id="916464963798167-footnote-ref-34"><a href="#916464963798167-footnote-34">[34]</a></sup></sup> etc.) for adding classification tags to your material and specify the vocabulary you use in the metadata record; give at least one broad category for your material (e.g. life sciences, computing etc.).
*   In all cases, where linking to other resources or entities (e.g. persons, projects etc.) in the metadata records is added, please try to do this through unique and persistent identifiers of authority lists and sources, to the extent possible, documenting also the authority and/or scheme it adheres to.

The following sections include a synopsis of the minimal schemas<sup><sup id="916464963798167-footnote-ref-35"><a href="#916464963798167-footnote-35">[35]</a></sup></sup> for ancillary knowledge resources, i.e. the subset of M(andatory) and strongly R(ecommended) metadata elements per resource type, given that knowledge resources may take one of the following resource types:

*   **lexical/conceptual resource**: reserved not only for lexica, ontologies, term lists, glossaries etc. but also for any resource that can be used for annotation purposes, i.e. linguistic tagsets, typesystems etc.
*   **language description**: reserved mainly for computational grammars
*   **model**: for machine learning and statistical models.

It should also be noted that additional elements required for the management of the metadata record (e.g. _metadataCreationDate, metadataCreator_ etc.) are not presented here, as they are to be handled by the OMTD platform.

