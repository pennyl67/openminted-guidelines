#### contactPerson (identifier or personName)
##### Usage
Recommended
##### Type
identifier or multilingual free text
##### Attributes
ms:personIdentifierSchemeName (for identifiers) or xs:lang (for name)
##### Definition/Explanations
 Groups information on the person(s) that is/are responsible for providing further information regarding the resource
##### Recommended usage
The recommended way for referring to a person is by giving their identifier, preferably the ORCID; if you provide the identifier, please select also the relevant value from the list of values in the attribute "personIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 
If you don't know the identifier of the person, you may provide the name, preferably in the format "Surname, First name" at least in English; if you want to add names in other languages, you can use the “lang” attribute. 
The element can also be repeated to encode multiple persons. 
If you decide to add a contactPerson instead of a general contactEmail, please ensure that the data (including the email) of this person are also uploaded in OpenMinTeD.
##### Relation to other metadata schemas
* **DataCite 4.0:** contributor with datacite:contributorType="ContactPerson", *datacite:contributorName (familyName & givenName) or datacite:nameIdentifier and datacite:nameIdentifierScheme and datacite:schemeURI)
