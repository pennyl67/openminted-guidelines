#### relatedResource
##### Usage
Mandatory when applicable
##### Conditions for usage
when relationType is filled in
##### Type
ms:resourceIdentifierSchemeName or ms:schemeURI (for identifiers) and xs:lang (for names)
##### Definition/Explanations
A name or an identifier (e.g. url reference) to the target resource related through a relation encoded in relationType 
##### Recommended usage
The recommended way for referring to a resource is by giving its name and optionally its identifier; if you provide the identifier, please select also the relevant value from the list of values in the attribute "resourceIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 

Annotated corpora must be linked to the raw corpus (as relatedResource) through the relationType with value isAnnotatedVersion.

For interoperability reasons, it is recommended to describe all related resources in the OpenMinTeD registry and refer to them through the identifier.
