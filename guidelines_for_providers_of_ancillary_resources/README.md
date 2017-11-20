# Guidelines for providers of knowledge resources \(ML models, grammars and annotation resources\) {#guidelines-for-providers-of-ancillary-knowledge-resources}

A lot of TDM applications and components make use of _**ancillary knowledge resources**_. By knowledge resources, we mean information from some domain or area of human endeavor \(e.g. linguistics, agriculture, or the social sciences\), represented in a form that can be used to solve problems computationally in that domain or area[^1]. Creation of such knowledge resources is widespread in both linguistics, and in many domains where informatics is applied. These knowledge resources typically include controlled vocabularies, terminologies, lexica, ontologies, and so on.

As OpenMinTeD is about applying TDM to end-user domains, the _**resources used in those domains**_ are of primary importance. Similarly, as text is important to OpenMinTeD tools and services, so _**linguistic resources**_ \(e.g. resources that describe parts of speech\) are also important.

OpenMinTeD tools and services may make use of these resources in order to annotate text. For example, an application may make use of a dictionary of archaeological terms when processing object descriptions. Or, another application may make use of parts of speech to find the adjectives in a document, and use this information to help determine the sentiment of the document. To indicate this, the term _**annotation resource **_ is introduced as a cover term.

Another type of knowledge resource used by tools and services during processing are _**grammars**_ and _**Machine Learning models**_ that help analyse the text. The choice depends upon the approach of the component.

![](/assets/5a.png)

In order to make it easier to share the results of TDM, and in order to allow TDM components to work together, OpenMinTeD makes a number of [_**recommendations**_** **](/recommendations-for-publishers.md)about how knowledge resources are represented. Knowledge resources that do not follow these recommendations can of course be used; however, interoperability will be reduced.

The OpenMinTeD recommendations on knowledge resources are based on the [**Linked Data**](https://www.w3.org/standards/semanticweb/data) paradigm. By "Linked Data", we mean data that is created and made available with the use of semantic web technologies and formats \(e.g. RDF, OWL, SPARQL\) and, most importantly, that is interrelated with other data.

---

[^1]: Poole, David and Alan Mackworth \(2010\) _Artificial Intelligence_, Cambridge University Press

