## How to comply with OpenMinTeD interoperability specifications

In order to make it easier to share the results of TDM, and in order to allow TDM components and applications to work together and interact appropriately with ancillary knowledge resources, OpenMinTeD makes a number of [_**recommendations**_](/guidelines_for_providers_of_ancillary_resources/how-to-make-your-knowledge-resources-interoperable.md) about how knowledge resources are represented. Knowledge resources that do not follow these recommendations can of course be used; however, interoperability will be reduced.

###Technical recommendations 
The OpenMinTeD recommendations on annotation resources are based on the [**Linked Data**](https://www.w3.org/standards/semanticweb/data) paradigm. By "Linked Data", we mean data that is created and made available with the use of semantic web technologies and formats \(e.g. RDF, OWL, SPARQL\) and, most importantly, that is interrelated with other data.

For ML models and grammars, the main technical recommendations come from the requirements that the apps/components themselves pose on them.

More specifically:
* **for annotation resources**:
  * **Data formats**: you must provide the resource in a standard format, preferably XML or JSON-based syntax, or any other RDF serialisation format \(e.g. Turtle or N3\)
  * **Identifiers**: all elements in the knowledge resource must be identified with a URI; for Linked Data resources, the following identifiers should be used:
    * JSON-LD - the @id keyword
    * RDF/XML - the attributes xml:base, rdf:ID and rdf:about
    * XML - the xml:id attribute
* **for ML models**:
  * you must register them independently of any component that uses them, e.g. in a separate Maven artifact
  * **Data formats**: you must provide the resource in a format compatible with the app/component that will deploy it; the value of the format must be declared in the metadata element _dataFormat_
  
###Other recommendations 
If you want to be fully compliant with the OpenMinTeD interoperability requirements, please ensure that you adopt the following rules; if you fail to abide to them, it might still be possible to operate your software resources via the OpenMinTeD platform, but this cannot be guaranteed and interoperability with other resources will suffer loss.

To be fully compatible with OpenMinTeD, you must 
* **Licensing**
  * Please, ensure that the resource is distributed under _**Open Access conditions**_
  * You must include in the metadata record a _**link to the licence**_ document that describes the terms and conditions under which it is provided, and attach the licence document together with the resource
  
{% blurb style='tip'%}
Please note that 
* using a standard licence, such as [Creative Commons](https://creativecommons.org/share-your-work/) the most recent version, is recommended for annotation resources
* you can use the [licence compatibility matrix](https://openminted.github.io/releases/license-matrix/) to check whether your resources can be combined with TDM applications/components
{% endblurb %}

* **Persistent and Unique identifiers:**
  * if you already have a PID for your resource (e.g. a URI or a HANDLE), make sure it is _**included in the metadata record**_ (cf. [identifier](/models_identifier.md) for more information)
* **Linked Data principles**: You must provide linkage between your resource and other resources (domain-specific or generic resources); for links between knowledge resources in the Linked Data paradigm, mapping should be expressed through RDF statements, using relations from [SKOS](https://www.w3.org/2004/02/skos/), together with the following OWL and RDF object properties: _owl:sameAs_, _owl:equivalentClass_, _owl:equivalentProperty_, _rdfs:subClassOf_, _rdfs:subPropertyOf_
*  **Versioning**: version all your resources and label the versions in an unambiguous way, preferably following the [Semantic Versioning recommendations](http://semver.org).
* **Documentation**: It is important that you provide the appropriate documentation for your resource (e.g. publications about the design and construction of the resource, etc.), which you should also version along with the knowledge resource and add as reference to your metadata record.
* **Citation**: 
  * Make sure that you fill in the metadata record_** all the elements required for citing your resource**_[^1], i.e. the creator of the resource, a title, the resource type and an identifier, and optionally, the publication date, the version and the publisher or distributor
  * You may _**recommend one of the publications**_ about your resource as the one to be cited for scholarly attribution and add this information in the metadata record.
* **Domain classification**: Use _**standard classification vocabularies **_(e.g. [MeSH](https://www.nlm.nih.gov/mesh/), [DDC](https://www.oclc.org/dewey.en.html), [LCSH](http://id.loc.gov/authorities/subjects.html) etc.) for adding classification tags to your material and specify the vocabulary you use in the metadata record; provide at least one broad category for your material (e.g. life sciences, computing etc.).
* **Linking to other entities**: In all cases, where linking to other resources or entities (e.g. persons, projects etc.) in the metadata records is added, please try to do this _**through unique and persistent identifiers of authority lists and sources**_, to the extent possible, documenting also the authority and/or scheme it adheres to.

******
[^1] For citation, OpenMinTeD endorses the [Joint Declaration of Data Citation Principles](https://www.force11.org/group/joint-declaration-data-citation-principles-final), as well as the more specialised [RDA recommendations for data citation of evolving data](https://www.rd-alliance.org/system/files/RDA-DC-Recommendations_151020.pdf) and [DataCite guidelines](https://www.datacite.org/cite-your-data.html).



