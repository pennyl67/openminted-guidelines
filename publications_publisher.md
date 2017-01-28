#### publisher
##### Usage
Recommended
##### Type
person or organization, both encoded with identifier or multilingual free text
##### Attributes
for person: ms:personIdentifierSchemeName (for identifiers) or xs:lang (for name); for organization: ms:organizationIdentifierSchemeName (for identifiers) or xs:lang (for name)
##### Definition/Explanations
 Groups information on the person(s) or organization(s) that has/have published the publication
##### Recommended usage
The recommended way for referring to a person is by giving their identifier, preferably the ORCID; if you provide the identifier, please select also the relevant value from the list of values in the attribute "personIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 
If you don't know the identifier of the person, you may provide the name, preferably in the format "Surname, First name" at least in English; if you want to add names in other languages, you can use the “lang” attribute. 
The recommended way for referring to an organization is by giving their identifier (e.g. ISNI); if you provide the identifier, please select also the relevant value from the list of values in the attribute "organizationIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 
If you don't know the identifier of the organization at least in English; if you want to add names in other languages, you can use the “lang” attribute. 
 The element can also be repeated to encode multiple persons/organizations.
##### Relation to other metadata schemas
* **OpenAIRE current version:** publisher
* **OpenAIRE v4.0:** dc:publisher
* **CORE:** article.publisher
* **DCMI:** skos:exactMatch dct:publisher
* **DataCite 4.0:** skos:exactMatch dct:Publisher
