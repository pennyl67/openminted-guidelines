#### contactPerson

##### Usage

Recommended

**Type**

set of elements

**Mandatory and recommended elements**

| **Element** | **Usage** |
| :--- | :--- |
| surname | Mandatory |
| givenName | Recommended |
| personIdentifier | Recommended |
| email | Mandatory for contact persons |
| affiliation: organizationName and organizationIdentifier | Recommended |

##### Attributes

ms:personIdentifierSchemeName \(for identifiers of persons\) and organizationIdentifierSchemeName \(for identifiers of organizations\)

##### Definition/Explanations

Groups information on the person\(s\) that is/are responsible for providing further information regarding the resource

##### Recommended usage

The recommended way for referring to a person is by giving their surname and given name\(s\) as well as their identifier\(s\), preferably the ORCID.  
If you provide the identifier, please select also the relevant value from the list of values in the attribute "personIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme.  
The element can also be repeated to encode multiple persons.

**Relation to other metadata schemas**

* **DataCite 4.0:** contributor with datacite:contributorType="ContactPerson", \*datacite:contributorName \(familyName & givenName\) or datacite:nameIdentifier and datacite:nameIdentifierScheme and datacite:schemeURI\)



