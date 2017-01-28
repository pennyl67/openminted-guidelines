#### tagset inside inputContentResourceInfo or outputResourceInfo
##### Usage
Mandatory when applicable
##### Conditions for usage
if the input content resource (i.e. the resource to be mined) or the output resource (the results of the processing) is to be described, this element is obligatory
##### Type
identifier or multilingual free text
##### Attributes
ms:resourceIdentifierSchemeName or ms:schemeURI (for identifiers) and xs:lang (for names)
##### Definition/Explanations
A name or an identifier (e.g. url reference) to the tagset used in the annotation of the resource or used by the component
##### Recommended usage
The recommended way for referring to a resource is by giving its identifier; if you provide the identifier, please select also the relevant value from the list of values in the attribute "resourceIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 
If you don't know the identifier of the resource, you may provide the name at least in English; if you want to add names in other languages, you can use the “lang” attribute. 
For interoperability reasons, it is recommended to describe typesystems, tagsets, annotation resources etc. in the OpenMinTeD registry and refer to them through the identifier.
