#### language
##### Usage
Mandatory
##### Type
open controlled vocabulary
##### Controlled vocabulary reference and/or values
ms:language (a combination of languageId, scriptId, regionId and variantId according to the IETF BCP47 guidelines): 
##### Definition/Explanations
The language(s) of the resource according to IETF BCP47 guidelines. 
##### Recommended usage
Please, enter the language and, if needed, the region, script and variant identifier that best fits the language used to describe the resource (e.g. en-US) according to the IETF BCP47 guidelines; not to be confused with "language" which is used for the language of the contents of the resource. 
For instance, a lexicon of English with definitions in English and French must be encoded with "language" "English" and 2 "metalanguage" values for "English" and "French". 
The element can be repeated for multiple languages.
##### Relation to other metadata schemas
* **DCMI:** skos:closeMatch dct:language
* **DataCite 4.0:** skos:closeMatch datacite:Language
