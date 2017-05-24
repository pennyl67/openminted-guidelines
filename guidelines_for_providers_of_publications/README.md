# Guidelines for providers of publications {#guidelines-for-providers-of-publications}

## Introduction {#introduction}

OpenMinTeD focuses on the use of TDM technologies in the scientific publications world, ranging from generic scholarly communication to literature related to specific disciplines. Scholarly publications come from a wide bulk of stakeholders, e.g. institutional and discipline repositories, academic journals, scientific publishers, etc. For the first phase, the focus is on **literature repositories and publishers**, as regards sources, and on **Open Access content**, as regards access conditions.

OpenMinTeD relies on existing infrastructures and standards/best practices for its operation. Thus, to access scholarly publications, it relies on the two main aggregators of such content, [OpenAIRE](http://www.openaire.eu) and [CORE](http://core.ac.uk). 

To provide your resources in OpenMinTeD for TDM purposes, you can:
* deposit them through one of the aggregators, following their respective guidelines and procedures - for more information, see ~~link~~,
* provide them through your API, using the content connector that has been built in the OpenMinTeD framework that allows harvesting of open access publications through the APIs of publishers that allow this. ~~further info or requirements for this??~~

### Deployment of publications in OpenMinTeD {#Deployment of publications in OpenMinTeD}
Scholarly publications are imported into OpenMinTeD for TDM processing via _**the creation of corpora upon queries submitted by the end-users**_. 
Researchers can build a corpus by selecting publications from various sources based on specific criteria, e.g. "a corpus of English articles in the biomedicine area", in order to run TDM services on them. 

OpenMinTed has elaborated several architectural options of how to integrate existing content providers (such as OpenAIRE and CORE but not limited to) and choose an approach whereby content is managed in those external services but is accessible in the OpenMinTeD platform through a **federated search strategy**. Content is made available to OpenMinTed platform through a simple API, defining simple operations to search and retrieve content. 

As one of the first steps of building a corpus of scholarly publications, end-users are expected to issue a query in the OpenMinTed registry; in fact, they are presented with a faceted view of the OpenMinTeD contents \(i.e. of all registered content providers\) and, by selecting from a range of criteria, a query is gradually built. Results from all registered content providers are presented to the end-user and, after refinement and careful elicitation of the final query, the associated content is transferred to OpenMinTeD’s registry and becomes available for the subsequent steps of a TDM workflow. A lazy deposit/caching strategy has been employed to avoid redundant queries (in simple terms, a record is fetched only the first time it is requested and remains persistent locally for further requests). Extra care is taken to ensure reproducibility of the created corpus by storing an exact version of the content used in it.

Thus, a corpus included in the OpenMinTeD Registry essentially consists of a list of publications. Each publication is identified (equivalent to a primary key) by its content (full text pdf) hash vialue and a set of metadata files (compatible with the OMTD-SHARE schema) that describe the resource. In most cases, this set consists of just one item; still, it cannot be ruled out that the same resource is described by multiple metadata files (for example, different metadata files from CORE or OpenAIRE, updates in metadata fields, richer metadata from a content provider, etc.) 

T**he ingredients, therefore, that are essential for providing publications into OpenMinTeD are**:
* the **full text** of the publication in a format that can be processed (see link)
* a **metadata description** of the publication with the elements that are used as criteria for the user queries; the metadata must be compatible with the OMTD-SHARE schema;   mappings from the OpenAIRE and CORE schemas are also provided.



* [Introduction](/introductory-remarks.md)
* [Instructions for publication repositories, libraries, publishers etc.](/guidelines_for_providers_of_publications/instructions_for_publication_repositories_librari.md)
* [Instructions for aggregators](/guidelines_for_providers_of_publications/instructions_for_aggregators.md)
* [Further requirements for annotated publications](/guidelines_for_providers_of_publications/further-requirements-for-annotated-publications.md)
* [Recommended schema for publications](/guidelines_for_providers_of_publications/recommended_schema_for_publications.md)



