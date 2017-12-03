# The OMTD-SHARE metadata schema {#the-omtd-share-metadata-schema}

The **OMTD-SHARE metadata schema**[^1] is the recommended schema for the description of the resources. It has been conceived and designed in order to serve as a facilitator, providing the interoperability bridge between the various resource types involved in TDM processes, and as an intermediary with the target audience, including TDM developers and end-users.

![](/assets/OMTD_Schemav2OverviewNewcolors2.jpg)

Its design takes into consideration the fact that both resources and users come from different scientific communities and tries to achieve interoperability through a _**common core vocabulary**_** **for the description of resources and their properties, establishing links to the vocabularies already used by the various sources for this purpose. Standards and best practices of the source communities are taken aboard to the best extent possible. The main principles and strategies employed in the design of the OMTD-SHARE schema consist of the following:

* cover needs of resource discoverability and TDM processing
* cover documentation needs of all resource types involved in TDM
* be flexible enough to support varying degrees of documentation completeness
* organize the schema elements and accommodate common vs. particular features of resources
* reuse what is available vs. create and recommend new elements and values
* standardize/normalize user input vs. allow for free user input
* document processing procedure and outputs.

It has largely been based on the [META-SHARE metadata schema](http://metashare.ilsp.gr/knowledgebase/homePage) \[Gavrilidou et al. 2012\], which caters for the description of language resources, encompassing both data \(textual, multimodal/multimedia and lexical data, grammars, language models etc.\) and technologies \(tools/services\) used for their processing. The OMTD-SHARE is more restricted in the sense that it focuses on text resources only, while it also extends the basic schema in order to include TDM-specific concepts, and describe in an enhanced way processing procedures and workflows.

As in META-SHARE, the schema sets out to document the full lifecycle of a resource, which also includes at least a minimal documentation of the satellite entities that participate in it, especially the relations that hold between them. The OMTD-SHARE data model thus comprises of the following entities:

* the _**resources**_, further classified into:
  * _**corpora**_, i.e. datasets of text documents - mainly scholarly publications in OMTD-SHARE
  * _**lexical/conceptual resources**_, including lexica, ontologies, term lists, gazetteers etc., but also tagsets and annotation schemas, which are used for annotating corpora - hence also called _**annotation resources **_in the OpenMinTeD context
  * _**language descriptions**_, which mainly refer to computational grammars and machine learning and statistical _**models**_[^2],
  * software _**components**_, pieces of software, tools offered as locally executable codes or as web services, wrapped in a workflow or as standalone end-to-end applications, and, finally,
  * _**publications**_, which constitute a peculiar resource type, as they are viewed in OpenMinTeD only in a collective form, as a "corpus",
* but also satellite entities, such as the _**actors**_, be it _**persons**_** **or _**organizations**_** **that have created the resources, or the _**projects**_** **that have funded them or where they are used.

Obviously, lexical/conceptual resources, language descriptions and models are ancillary resources used for the TDM operation. Corpora are an in-between case as they may refer to corpora used for the TDM operation, such as training or evaluation corpora and thus play a supportive role, or they can be composed of scholarly publications, in which case they are approached as a proper content resource to be mined.

The schema is composed of metadata elements that are used to describe properties and relations between all these entities. Some of these elements, especially those that pertain to administrative features \(e.g. identification, contact, licensing information etc.\), are common to all types of resources, while other elements, mainly those representing technical features about the contents and format of resources, differ across types. As aforesaid, publications differ from other resources types: the metadata elements recommended for their description mainly derive from the need of serving as selection criteria in the corpus building process.

One of the characteristic features of the SHARE family of schemas[^3] is the adoption of the component-based mechanism \(Component MetaData Infrastructure, CMDI\), according to which semantically coherent elements are grouped together to form components[^4] \[Broeder et al., 2008\]. For instance, the licensing module includes elements such as the name and URL of a licence, attribution text, copyright holders, etc. For the sake of simplification, the container elements used for this grouping will not be presented in the guidelines unless required.

The OMTD-SHARE schema classifies elements into three levels of optionality:

* _**mandatory**_: elements that are necessary for intended purposes, i.e. for discovering resources and for triggering operations between content and software
* _**recommended**_: elements that can help the current or future use of the resource, or useful information that providers have not yet standardized
* _**optional**_: all remaining information related to the lifecycle of a resource.

The schema is currently implemented as an XSD[^5]. An important difference from META-SHARE lies in the organisation vis-a-vis the different resource types covered: while META-SHARE describes all resources types in one common XSD, in OMTD-SHARE, the resource types are described in a more modular way as separate sets of XSDs.

The current version of the schema makes use of the OMTD-SHARE ontology, which caters for:

* annotation types
* data formats
* component and application types.

The OMTD-SHARE ontology will continue to evolve in order to take into account the emerging needs for registering new TDM components and applications.

[^1]: The full OMTD-SHARE schema is documented at: [https://openminted.github.io/releases/omtd-share/](https://openminted.github.io/releases/omtd-share/).

[^2]: In the first version of the schema, ML models were added as a distinct resource type, but in v2.0.0 they have been added as a subtype of language descriptions.

[^3]: Based on the META-SHARE schema, four more adaptations are now available:  [ELRC-SHARE](https://www.elrc-share.eu/documentation/elrcShareSchema.html), [clarin:el](http://www.clarin.gr/en/content/preparing-documenting-lrs), [retele-share](http://ontoology.linkeddata.es/publish/retele-share/index-en.html) and OMTD-SHARE. The META-SHARE schema has also been implemented as an [RDF/OWL ontology](http://purl.org/net/def/metashare) with the collaboration of the [ld4lt](https://www.w3.org/community/ld4lt) W3C group.

[^4]: To avoid confusion with the term "component" also used for software components, we will from now on refer to this concept as "modules".

[^5]: You can find the latest and previous versions of XSD's and full documentation at: [https://openminted.github.io/releases/omtd-share/](https://openminted.github.io/releases/omtd-share/)

