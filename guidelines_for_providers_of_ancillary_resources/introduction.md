## Introduction {#introduction}

Many TDM tools and services make use of **_ancillary knowledge resources_**. By knowledge resources, we mean information from some domain or area of human endeavor (e.g. linguistics, agriculture, or the social sciences), represented in a form that can be used to solve problems computationally in that domain or area[^1]. Creation of such knowledge resources is widespread in both linguistics, and in many domains where informatics is applied. These knowledge resources typically include controlled vocabularies, terminologies, lexica, ontologies, and so on.

As OpenMinTeD is about applying TDM to end-user domains, the resources used in those domain are of primary importance. Similarly, as text is important to OpenMinTeD tools and services, so linguistic resources (e.g. resources that describe parts of speech) are also important.

OpenMinTeD tools and services may make use of these resources in order to process text. For example, a service may make use of a dictionary of archaeological terms when processing object descriptions. Or, a service may make use of parts of speech to find the adjectives in a document, and use this information to help determine the sentiment of the document.

In order to make it easier to share the results of TDM, and in order to allow TDM tools and services to work together, OpenMinTeD makes a number of **_recommendations_ **about how knowledge resources are represented. Knowledge resources that do not follow these recommendations can of course be used; however, interoperability will be reduced.

The OpenMinTeD recommendations on knowledge resources are based on the **[Linked Data](https://www.w3.org/standards/semanticweb/data)** paradigm. By &quot;Linked Data&quot;, we mean data that is created and made available with the use of semantic web technologies and formats (e.g. RDF, OWL, SPARQL) and, most importantly, that is interrelated with other data.

************************
[^1]: Poole, David and Alan Mackworth (2010) _Artificial Intelligence_, Cambridge University Press
