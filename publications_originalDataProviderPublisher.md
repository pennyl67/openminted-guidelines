#### originalDataProviderPublisher
##### Usage
Recommended when applicable
##### Conditions for usage
if originalDataProviderType=publisher
##### Type
organization encoded with identifier or multilingual free text
##### Attributes
ms:organizationIdentifierSchemeName (for identifiers) or xs:lang (for name)
##### Definition/Explanations
Refers to the publisher from which the metadata record has been harvested
##### Recommended usage
The recommended way for referring to an organization is by giving their identifier (e.g. ISNI); if you provide the identifier, please select also the relevant value from the list of values in the attribute "organizationIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 
If you don't know the identifier of the organization at least in English; if you want to add names in other languages, you can use the “lang” attribute.
##### Relation to other metadata schemas
* **OpenAIRE current version:** collectedFrom
* **DCMI:** skos:narrowMatch dct:source
