#### characterEncoding inside inputContentResourceInfo or outputResourceInfo
##### Usage
Mandatory when applicable
##### Conditions for usage
if the input content resource (i.e. the resource to be mined) or the output resource (the results of the processing) is to be described, this element is obligatory
##### Type
open controlled vocabulary
##### Controlled vocabulary reference and/or values
ms:characterEncoding: a long list of popular character encodings

##### Definition/Explanations
The name of the character encoding used in the resource or supported by the component
##### Recommended usage
Please, select one of the pre-defined values; it should be noted, however, that for OpenMinTeD the preferred character encoding is UTF-8 to ensure interoperability between content and components. 
The element can be repeated for components that support various character encodings.
##### Relation to other metadata schemas
* **GATE:** Parameters/encoding
