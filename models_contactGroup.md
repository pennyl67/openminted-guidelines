#### contactGroup
##### Usage
Recommended
##### Type
identifier or multilingual free text
##### Attributes
ms:organizationIdentifierSchemeName (for identifiers) or xs:lang (for name)
##### Definition/Explanations
 Groups information on the group(s) that is/are responsible for providing further information regarding the resource
##### Recommended usage
The recommended way for referring to a group (currently modelled as an organization) is by giving their identifier (e.g. ISNI, fundref); if you provide the identifier, please select also the relevant value from the list of values in the attribute "organizationIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 
If you don't know the identifier of the group (organization), you may provide the name at least in English; if you want to add names in other languages, you can use the “lang” attribute. 
If you decide to add a contactGroup instead of another contact option, please ensure that the data (including the communication data) of this group (organization) are also uploaded in OpenMinTeD.
