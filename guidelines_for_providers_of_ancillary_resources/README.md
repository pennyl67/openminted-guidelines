# Guidelines for providers of knowledge resources \(ML models, grammars and annotation resources\)

We welcome knowledge resources that can be used together with components/applications hosted by OpenMinTeD in order
* to annotate content or
* to help analyse it.

![](/assets/5a.png)

##What we mean with "knowledge resources"
A lot of TDM applications and components make use of _**ancillary knowledge resources**_. 

By "knowledge resources", we mean information from some domain or area of human endeavor \(e.g. linguistics, agriculture, or the social sciences\), represented in a form that can be used to solve problems computationally in that domain or area[^1]. Creation of such knowledge resources is widespread in both linguistics, and in many domains where informatics is applied. These knowledge resources typically include controlled vocabularies, terminologies, lexica, ontologies, and so on.

OpenMinTeD applications and components may make use of these resources in order to **annotate text**. For example, an application may make use of a dictionary of archaeological terms when processing object descriptions. Or, another application may make use of parts of speech to find the adjectives in a document, and use this information to help determine the sentiment of the document. To indicate this, the term _**annotation resource **_ is introduced as a cover term.

Another type of knowledge resource used by applications and components during processing are _**grammars**_ and _**Machine Learning models**_ that help analyse the text. The choice depends upon the approach of the app/component.

##OpenMinTeD focus on knowledge resources
As OpenMinTeD is about applying TDM to domains of interest of the end-users, the _**resources used in these domains**_ are of primary importance. Similarly, as text is important to OpenMinTeD applications, so _**linguistic resources**_ \(e.g. resources that describe parts of speech\) are also important.

## Conditions for sharing knowledge resources
If you wish to share ancillary knowledge resources through the [OpenMinTeD platform](https://services.openminted.eu/home), you must

* ensure that your resource adheres to **at least the minimal level of the [OpenMinTeD interoperability specifications](/guidelines_for_providers_of_ancillary_resources/how-to-make-your-knowledge-resources-interoperable.md)**,

* provide access to the ** actual contents** of the resource, and

* add in the OpenMinTeD registry, according to the [relevant instructions](/guidelines_for_providers_of_ancillary_resources/instructions_for_providers_of_ancillary_knowledge.md), the [annotation resource](https://services.openminted.eu/resourceRegistration/lexical) or the [ML model/grammar](https://services.openminted.eu/resourceRegistration/language) with a **metadata record **compliant with at least the [minimal OMTD-SHARE schema](/recommended-metadata-for-knowledge-resources.md).


---

[^1]: Poole, David and Alan Mackworth \(2010\) _Artificial Intelligence_, Cambridge University Press

