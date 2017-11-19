#### contactGroup

##### Usage

Recommended

##### Type

set of elements

**Mandatory and recommended elements**

| **Element** | **Usage** |
| :--- | :--- |
| groupName | Mandatory |
| affiliation: organizationName and organizationIdentifier | Recommended |

##### Attributes

ms:organizationIdentifierSchemeName \(for identifiers\) or xs:lang \(for name\)

##### Definition/Explanations

Groups information on the group\(s\) that is/are responsible for providing further information regarding the resource

##### Recommended usage

The recommended way for referring to a group is by giving their name \(e.g. "Software development team"\) and the name and \(optionally\) the identifier \(e.g. ISNI, fundref\) of the affiliated organization. An email address is also recommended.

If you provide the identifier of the organization, please select also the relevant value from the list of values in the attribute "organizationIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme.

##### Relation to other metadata schemas

* **Maven POM 4.0.0:** developers



