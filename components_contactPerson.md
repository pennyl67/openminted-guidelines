#### contactPerson

##### Usage

Recommended

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

The recommended way for referring to a person is by giving their surnames and given names and supplying also their unique identifiers, preferably the ORCID; if you provide the identifier, please select also the relevant value from the list of values in the attribute "personIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme.  
If you provide the name as a single element \(personName\), please use the format "Surname, First name".  
The element can also be repeated to encode multiple persons.  
If you decide to add a contactPerson instead of a general contactEmail, please ensure that the data \(including the email\) of this person are also uploaded in OpenMinTeD.

##### Relation to other metadata schemas

* **DataCite 4.0:** contributor with datacite:contributorType="ContactPerson", \*datacite:contributorName \(familyName & givenName\) or datacite:nameIdentifier and datacite:nameIdentifierScheme and datacite:schemeURI\)



