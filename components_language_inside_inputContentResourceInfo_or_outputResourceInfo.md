#### language inside inputContentResourceInfo or outputResourceInfo
##### Usage
Mandatory when applicable
##### Conditions for usage
if the input content resource (i.e. the resource to be mined) or the output resource (the results of the processing) is to be described, this element is obligatory
##### Type
open controlled vocabulary
##### Controlled vocabulary reference and/or values
ms:language (a combination of languageId, scriptId, regionId and variantId according to the IETF BCP47 guidelines): 
##### Definition/Explanations
The language(s) of the text that the component supports (takes as input and/or produces), expressed according to IETF BCP47 guidelines. The element can be repeated to encode multiple languages. 
##### Recommended usage
Please, enter the language and, if needed, the region, script and variant identifier that best fits the language of the document (e.g. en-US) that the component supports (takes as input and/or produces), expressed according to the IETF BCP47 guidelines. 
The element can be repeated for components that support various character encodings.
##### Relation to other metadata schema elements
* **UIMA/UIMA-fit:** @LanguageCapability
* **DataCite 4.0:** language - but this is the language of the resource and not of input/output
