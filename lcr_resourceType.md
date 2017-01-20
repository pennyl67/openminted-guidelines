#### resourceType
##### Usage
Mandatory
##### Type
Closed controlled vocabulary
##### Controlled vocabulary reference and/or values
ms:resourceType: _corpus_, _lexicalConceptualResource_, _languageDescription_, _model_, _component_
##### Definition/Explanations
Specifies the type of the resource being described or the type of the resource that a component takes as input or produces as output
##### Recommended usage
For lexical/conceptual resources, the fixed value "lexicalConceptualResource" must be added automatically
##### Relation to other metadata schema elements
* **DCMI:** skos:narrowMatch dct:type
* **DataCite 4.0:** skos:closeMatch datacite:resourceTypeGeneral & datacite:resourceType; recommended usage for lexical/conceptual resources is to use "dataset" but the values "collection" and "text" can also be used
