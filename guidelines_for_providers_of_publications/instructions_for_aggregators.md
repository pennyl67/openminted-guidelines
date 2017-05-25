## ​Instructions for providing publications directly into OpenMinTeD {#instructions-for-openaire-and-core}

For the first phase of the project, OpenAIRE and CORE will bring content resources into OpenMinTeD through user queries. For next versions, interested content providers will be able to contribute directly to OpenMinTeD if they implement the following:

* Map the metadata of their contents to the OMTD-SHARE schema
* Provide search capabilities on the metadata
* Provide the actual content \(e.g. fulltext in the case of publications\)

### How to connect to OpenMinTeD

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

For further requirements and recommendations that ensure compatibility of publications with OpenMinTeD tools and services, please see here.


---

[^1]: The OpenAIRE schema and guidelines are currently under revision; collaboration with the relevant actors has been established to take into account the new features and, where desired, influence the changes so as to support TDM processes in accordance to the interoperability requirements.

[^2]: Mappings with other metadata schemas, including OpenAIRE and CORE, are included in the presentation of the recommended metadata schema.



