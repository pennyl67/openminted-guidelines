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
* **Maven POM 4.0.0:** developers
* **DCMI:** skos:closeMatch dct:creator
* **DataCite 4.0:** creator with creatorName or nameIdentifier & nameIdentifierScheme & schemeURI; N.B. creatorName familyName & givenName in v4
