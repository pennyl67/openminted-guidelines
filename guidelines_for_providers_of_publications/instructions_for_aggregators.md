## ​Instructions for aggregators {#instructions-for-openaire-and-core}

For the first phase of the project, OpenAIRE and CORE will bring content resources into OpenMinTeD through user queries. For next versions, interested content providers will be able to contribute directly to OpenMinTeD if they implement the following:

* Map the metadata of their contents to the OMTD-SHARE schema
* Provide search capabilities on the metadata
* Provide the actual content \(e.g. fulltext in the case of publications\)

### How to register your resources {#how-to-share-your-resources}

Interested content providers must implement a Java interface, called **ContentConnector**, which can be found at [https://github.com/openminted/content-connector-api](https://github.com/openminted/content-connector-api). The implementation is then included in the code of the ContentService of the OpenMinTeD platform. This interface specifies three methods:

* _**search**_, which accepts a Query object describing a query and returns a page of metadata. This method is used for browsing the metadata of the provider and supports keyword search, advanced search in a number of fields and also faceted search. The result of the method is \(a\) a page \(of user specified size\) of metadata, \(b\) the statistics of the results \(total number of hits, etc\), and \(c\) the facets \(if requested\).

* _**fetchMetadata**_, which accepts a Query, but, unlike the previous method, returns all the metadata of the result, without any statistics or facets. The result is a stream containing a single xml element \(called “publications”\), which in turn contains all the metadata of the content. This method is called when a corpus is being built.

* _**downloadFullText**_, which given a publication identifier \(as contained in the metadata\) returns a stream containing the actual content. This method is again used when the platform is building a corpus.

Additional technical information is provided in the Java code of the interface.

### Minimal requirements

For each publication, you must deliver:
* a file with the **full text** 
* a **metadata description** with a minimal set of metadata elements in compliance with the OMTD-SHARE schema for publications and in XML format.

(see [here](/deployment-scenario-of-publications-in-openminted.md) for more information on the deployment of publications in OpenMinTeD).

It should be noted that the original resource providers \(e.g. publication repositories, publishers etc.\) that offer publications via OpenAIRE and CORE do not have to change their current schemas. Mappings and conversions between the OpenAIRE[^1] and CORE metadata and the OMTD-SHARE schema are made by the providers themselves in the framework of OpenMinTeD[^2].

To be fully compatible with OpenMinTeD, you must
* ensure that the publications are distributed under Open Access conditions
* include in the metadata record of each publication a link to the licence document that describes the terms and conditions under which it is provided, and attach the licence document together with the publication
* if you already have a PID for your publication \(preferably DOI\), make sure it is included in the metadata record \(cf. [identifier](/publications_identifier.md) for more information on identifier schemes\).


### Further recommendations
If you wish your material to be easily processable and interoperable with TDM tools and services, you should adopt the following recommendations:

* The preferred **formats** for delivering textual material are plain text, XML, PDF \(not proprietary and certainly not of scanned images\), which can be read by one of the existing readers.

* If appropriate for your material, use one of the **more specific data formats** that are already supported by readers and converters included in the OpenMinTeD registry \(cf. [dataFormat](/publications_dataFormat.md)\).

* The preferred **character encoding** is UTF-8.

* Further adoption of standards such as the [JATS article tag suite](https://jats.nlm.nih.gov/index.html) or [TEI P5 guidelines](http://www.tei-c.org/Guidelines/P5/) for annotating the inner structure of publications is recommended.

* Use standard classification vocabularies, such as [MeSH](https://www.nlm.nih.gov/mesh/), [DDC](https://www.oclc.org/dewey.en.html), [LCSH](http://id.loc.gov/authorities/subjects.html) etc.\) for adding classification tags to your material and specify the vocabulary you use in the metadata record; provide at least one broad category for your material \(e.g. life sciences, computing etc.\).

* In all cases, where linking to other resources or entities \(e.g. persons, projects etc.\) in the metadata records is added, please try to do this through unique and persistent identifiers of authority lists and sources, to the extent possible, documenting also the authority and/or scheme it adheres to.

Please, note that not all of the above requirements are absolute: if your material is not compliant with them, it may still be processable, but their adoption makes it better equipped for TDM and NLP processing.

---

[^1]: The OpenAIRE schema and guidelines are currently under revision; collaboration with the relevant actors has been established to take into account the new features and, where desired, influence the changes so as to support TDM processes in accordance to the interoperability requirements.

[^2]: Mappings with other metadata schemas, including OpenAIRE and CORE, are included in the presentation of the recommended metadata schema.



