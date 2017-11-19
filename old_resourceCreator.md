#### resourceCreator \(person or organization\)

##### Usage

Recommended

##### Type

person or organization

##### Attributes

for person: ms:personIdentifierSchemeName \(for identifiers\) or xs:lang \(for name\); for organization: ms:organizationIdentifierSchemeName \(for identifiers\) or xs:lang \(for name\)

##### Definition/Explanations

Groups information on the person\(s\) or organization\(s\) that has/have created the resource

##### Recommended usage

The recommended way for referring to a person is by giving their surname(s) and given name\(s\) as well as their identifier(s), preferably the ORCID.
If you provide the identifier, please select also the relevant value from the list of values in the attribute "personIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme.  
You must provide surnames and given names (as separate elements or as a single element, preferably in the format "Surname, Given name") at least in English. If you want to add names in other languages, you can use the “lang” attribute.  

The recommended way for referring to an organization is by giving their name and unique identifier \(e.g. ISNI\); if you provide the identifier, please select also the relevant value from the list of values in the attribute "organizationIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme.

The element can also be repeated to encode multiple persons/organizations.

For corpora created through the OMTD corpus building process, the resource creator is considered to be the person that has put together the corpus through the user query.

##### Relation to other metadata schemas

* **DCMI:** skos:closeMatch dct:creator
* **DataCite 4.0:** creator with creatorName or nameIdentifier & nameIdentifierScheme & schemeURI; N.B. creatorName familyName & givenName in v4



