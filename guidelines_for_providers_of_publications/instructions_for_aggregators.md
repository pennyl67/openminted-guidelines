## How to share content directly to OpenMinTeD

If you are a **publisher or a repository of scholarly works** and wish to share your content directly to the [OpenMinTeD platform ](https://services.openminted.eu) instead of following the [procedure through aggregators](/guidelines_for_providers_of_publications/instructions_for_publication_repositories_librari.md), you can do so if you implement the following:

* Map the metadata of your contents to the [OMTD-SHARE schema](/the_omtd-share_metadata_schema.md)
* Provide search capabilities on the metadata, according to the specifications of the **ContentConnector** described below
* Provide the actual content \(i.e. the full text\).

{% blurb style='tip'%}
It should be noted that the providers \(e.g. publication repositories, publishers etc.\) that offer publications via OpenAIRE and CORE do not have to change their current schemas. Mappings and conversions between the OpenAIRE[^1] and CORE metadata and the OMTD-SHARE schema are made by the providers themselves in the framework of OpenMinTeD[^2].
{% endblurb %}


###Minimum requirements for single documents (publications)
For each publication, you must 
* ensure that you adhere to the minimal level of the [OpenMinTed Interoperability specifications](/guidelines_for_providers_of_publications/recommendations-for-publishers.md), 
* provide access to a file with the **full text** 
* deliver a **metadata description** with a minimal set of metadata elements in compliance with the [**OMTD-SHARE schema**](/the_omtd-share_metadata_schema.md) for publications and in XML format; the metadata elements are used for creating uniform facets for querying the entire set of publications uploaded in OpenMinTeD \(see [here](/deployment-scenario-of-publications-in-openminted.md) for more information on the deployment of publications in OpenMinTeD\).

### How to connect to OpenMinTeD
You must implement a Java interface, called **ContentConnector**, according to the instructions found at [https://github.com/openminted/content-connector-api](https://github.com/openminted/content-connector-api). Through this interface, your contents will be integrated in the [OpenMinTeD platform](https://services.openminted.eu).

The interface implements the operations of the corpus building process \(cf. [Federated content search and corpus building](/deployment-scenario-of-publications-in-openminted.md)\):

* querying for specific metadata  elements and retrieving their values with statistical information \(e.g. number of records satisfying the query criteria\), 
* retrieval of the metadata themselves in XML format 
* retrieval of the full texts of the pulications.

Additional technical information is provided in the Java code of the interface.

---

[^1]: The OpenAIRE schema and guidelines are currently under revision; collaboration with the relevant actors has been established to take into account the new features and, where desired, influence the changes so as to support TDM processes in accordance to the interoperability requirements.

[^2]: Mappings with other metadata schemas, including OpenAIRE and CORE, are included in the presentation of the recommended metadata schema.

