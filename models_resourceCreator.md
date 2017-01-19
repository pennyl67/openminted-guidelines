#### resourceCreator (person or organization, described with identifier or name)
##### Usage
Recommended
##### Type
identifier or multilingual free text
##### Attributes
for person: ms:personIdentifierSchemeName (for identifiers) or xs:lang (for name); for organization: ms:organizationIdentifierSchemeName (for identifiers) or xs:lang (for name)
##### Definition/Explanations
Groups information on the person(s) or organization(s) that has/have created the resource
##### Recommended usage
##### Relation to other metadata schema elements
* **DCMI:** skos:closeMatch dct:creator
* **DataCite 4.0:** skos:closeMatch datacite:Creator with datacite:creatorName (familyName & givenName) or datacite:nameIdentifier & datacite:nameIdentifierScheme & datacite:schemeURI
