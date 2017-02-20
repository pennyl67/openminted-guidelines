## Introductory remarks {#introductory remarks}

OpenMinTeD aspires to facilitate the use of TDM technologies in the scientific publications world, ranging from generic scholarly communication to literature related to specific disciplines. Scholarly publications come from a wide bulk of stakeholders, e.g. institutional and discipline repositories, academic journals, scientific publishers, etc. For the first phase, the focus is on literature repositories and publishers, as regards sources, and on Open Access content, as regards access conditions.



End-users that wish to run TDM services on specific content will be presented with a faceted view of the OpenAIRE and CORE contents; by selecting from a range of criteria, a query will gradually be built which will be transferred to the respective APIs and retrieve the metadata records and data files of the matching publications. It should be noted that



{% blurb style='tip', title='Important notice' %}

only publications that provide the full text or, at least, an abstract are candidate for inclusion in OpenMinTeD.{% endblurb %}



OpenMinTeD relies on existing infrastructures and standards/best practices for its operation. Thus, to access scholarly publications, it relies on the two main aggregators of such content, [OpenAIRE](/www.openaire.eu) and [CORE](/core.ac.uk). Providers of scholarly publications are asked to contribute their resources by depositing them at one of these stakeholders, following their respective guidelines and procedures. In addition, OpenAIRE and CORE are developing a content connector that allows harvesting of open access publications through the APIs of publishers that allow this.

Scholarly publications are imported into OpenMinTeD for TDM processing based on a procedure which involves the creation of corpora upon queries submitted by the end-users. Researchers don't come to OpenMinTeD to read one by one publications, but to build a corpus by selecting publications from various sources based on specific criteria, e.g. "a corpus of English articles in the biomedicine area", in order to run TDM services on them. 
OpenMinTed has elaborated several architectural options of how to integrate existing content providers (such as OpenAIRE and CORE but not limited to) and choose an approach that content is managed in those external services but is accessible in the OpenMinTeD platform through a federated search strategy. Content is made available to OpenMinTed platform through a simple API, defining simple operations to search and retrieve content. 

As one of the first steps of building a corpus of scholarly publications, end-users are expected to issue a query in the OpenMinTed registry: in fact, they are presented with a faceted view of the OpenMinTeD contents \(i.e. of all registered content providers\) and, by selecting from a range of criteria, a query is gradually built. Results from all registered content providers are presented to the end-user and, after refinement and careful elicitation of the final query, the associated content is transferred to OpenMinTeD’s registry and becomes available for the subsequent steps of a TDM workflow. A lazy deposit/caching strategy has been employed to avoid redundant queries (in simple terms a record is fetched only the first time it is requested and remains persistent locally for further requests). Extra care is taken to ensure reproducibility of the created corpus by storing an exact version of the content used in it.

![](/assets/contentConnector1.jpg)

Therefore, a corpus included in the OpenMinTeD Registry essentially consists of a list of publications. Each publication is identified (equivalent to a primary key) by its content (full text pdf) hash value and a set of metadata files (in the OMTD-SHARE schema) that describe the resource. In most cases, this set consists of just one item but the case that multiple metadata files describe the same resource is possible (for example different metadata files from CORE or OpenAIRE, update in metadata fields, richer metadata from a content provider, etc.) 

![](/assets/contentConnector2.jpg)

The following sections present a list of requirements and recommendations that publications must meet to interact with TDM resources.

