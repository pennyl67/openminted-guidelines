#### publicationIdentifier

##### Usage

Mandatory

##### Type

free text

##### Attributes

ms-omtd:publicationIdentifierSchemeName or ms-omtd:schemeURI

##### Definition/Explanations

Reference to a DOI \(recommended\) or any kind of identifier used for the publication

##### Recommended usage

Provide a unique identifier already assigned by an authoritative source; the preferred identifier for publications is DOI; you can use either

* the attribute "publicationIdentifierSchemeName" to specify the scheme, by selecting one of the pre-defined values \(e.g. DOI, ISBN etc.\) or,
* if the scheme is not listed among them, use the "other" value, use the attribute "schemeURI" to provide a link to the URI that documents the scheme it adheres to.
  ##### Relation to other metadata schemas
* **OpenAIRE current version:** doi/pmc/etc. identifiers
* **OpenAIRE v4.0:** dc:identifier
* **CORE:** article.id & article.identifiers
* **DCMI:** skos:closeMatch dct:identifier
* **DataCite 4.0:** datacite:contributor with skos:broadMatch datacite:identifier \(identifierType can only be DOI\)contributorType="ContactPerson", contributorName \(familyName & givenName\) or nameIdentifier and nameIdentifierScheme and schemeURI



