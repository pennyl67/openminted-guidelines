#### contactPerson

##### Usage

Mandatory under conditions

##### Conditions for usage

For contact information, the data of a contactPerson or an email or a landingPage must be provided

##### Type

set of elements

**Mandatory and recommended elements**

| Element | Usage |
| :--- | :--- |
| surname and givenNames or personName | Mandatory \(choice: one element must be encoded\) |
| personIdentifier | Recommended |
| email | Mandatory for contact persons |
| affiliation: organizationName and organizationIdentifier | Recommended |

##### Attributes

ms:personIdentifierSchemeName \(for identifiers of persons\) or xs:lang \(for names\) and organizationIdentifierSchemeName \(for identifiers of organizations\)

##### Definition/Explanations

Groups information on the person\(s\) that is/are responsible for providing further information regarding the resource

##### Recommended usage

The recommended way for referring to a person is by giving their surname(s) and given name\(s\) as well as their identifier(s), preferably the ORCID.
If you provide the identifier, please select also the relevant value from the list of values in the attribute "personIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme.  
You must provide surnames and given names (as separate elements or as a single element, preferably in the format "Surname, Given name") at least in English. If you want to add names in other languages, you can use the “lang” attribute.  
The element can also be repeated to encode multiple persons.

If you decide to add a contactPerson instead of a general contactEmail, please ensure that the data \(including the email\) of this person are also uploaded in OpenMinTeD.

##### Relation to other metadata schemas

* **DataCite 4.0:** contributor with datacite:contributorType="ContactPerson", \*datacite:contributorName \(familyName & givenName\) or datacite:nameIdentifier and datacite:nameIdentifierScheme and datacite:schemeURI\)



