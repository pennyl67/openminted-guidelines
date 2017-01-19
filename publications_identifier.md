#### identifier
##### Usage
Mandatory
##### Type
free text
##### Attributes
ms-omtd:publicationIdentifierSchemeName or ms-omtd:schemeURI
##### Definition/Explanations
Reference to a DOI (recommended) or any kind of identifier used for the publication
##### Recommended usage
Provide a unique identifier already assigned by an authoritative source; the preferred identifier for publications is DOI; you can use either
##### Relation to other metadata schema elements
* **OpenAIRE current version:** doi/pmc/etc. identifiers
* **OpenAIRE v4.0:** dc:identifier
* **CORE:** article.id & article.identifiers
* **DCMI:** skos:closeMatch dct:identifier
* **DataCite 4.0:** datacite:contributor with skos:broadMatch datacite:identifier (identifierType can only be DOI)contributorType="ContactPerson", contributorName (familyName & givenName) or nameIdentifier and nameIdentifierScheme and schemeURI
