## Sharing scientific literature directly into OpenMinTeD \(Instructions for aggregators\) {#instructions-for-openaire-and-core}

For the first phase of the project, [**OpenAIRE**](https://www.openaire.eu/) and [**CORE**](https://core.ac.uk/) are responsible for bringing content resources into OpenMinTeD. In the upcoming versions, interested content providers will be able to contribute directly to OpenMinTeD if they implement the following:

* Map the metadata of their contents to the [OMTD-SHARE schema](/the_omtd-share_metadata_schema.md)
* Provide search capabilities on the metadata, according to the specifications of the **ContentConnector **\(cf. below\)
* Provide the actual content \(i.e. at least abstract or, preferably, full text\)

It should be noted that the providers \(e.g. publication repositories, publishers etc.\) that offer publications via OpenAIRE and CORE do not have to change their current schemas. Mappings and conversions between the OpenAIRE[^1] and CORE metadata and the OMTD-SHARE schema are made by the providers themselves in the framework of OpenMinTeD[^2].

For further requirements and recommendations that ensure compatibility of publications with OpenMinTeD tools and services, please see [here](/recommendations-for-publishers.md).

### How to connect to OpenMinTeD

Interested content providers must implement a Java interface, called **ContentConnector**, according to the instructions found at [https://github.com/openminted/content-connector-api](https://github.com/openminted/content-connector-api). Through this interface, their contents will be integrated in the OpenMinTeD platform.

The interface implements the operations of the corpus generation process \(cf. [deployment of publications in OpenMinTeD](/deployment-scenario-of-publications-in-openminted.md)\):

* querying for specific metadata  elements and retrieving their values with statistical information \(e.g. number of records satisfying the query criteria\), 
* retrieval of the metadata themselves in XML format 
* retrieval of the full texts of the pulications.

Additional technical information is provided in the Java code of the interface.

### Minimal requirements

For each publication, you must deliver:

* a file with the **full text** 
* a **metadata description** with a minimal set of metadata elements in compliance with the [**OMTD-SHARE schema**](/the_omtd-share_metadata_schema.md) for publications and in XML format; the metadata elements are used for creating uniform facets for querying the entire set of publications uploaded in OpenMinTeD \(see [here](/deployment-scenario-of-publications-in-openminted.md) for more information on the deployment of publications in OpenMinTeD\).



---

[^1]: The OpenAIRE schema and guidelines are currently under revision; collaboration with the relevant actors has been established to take into account the new features and, where desired, influence the changes so as to support TDM processes in accordance to the interoperability requirements.

[^2]: Mappings with other metadata schemas, including OpenAIRE and CORE, are included in the presentation of the recommended metadata schema.

