#### outputContentResourceInfo

##### Usage

Mandatory when applicable

##### Type

set of elements

##### Mandatory and recommended elements

| **Element** | **Usage** | **Type** |
| :--- | :--- | :--- |
| processingResourceType | Mandatory | closed controlled vocabulary |
| dataFormat \(& dataFormatOther\) | Mandatory when applicable | open controlled vocabulary |
| language | Mandatory when applicable | closed controlled vocabulary |
| annotationType \(& annotationTypeOther\) | Mandatory when applicable | open controlled vocabulary |

##### Definition/Explanations

Groups together information on the features set on the output resource of an application or component.

* **processingResourceType**: the  type of the resource used as input or produced by ouptut; values are _corpus, document, userInputText, lexicalConceptualResource, language Description_; e.g. readers that take as input a corpus, trainers that take as input a corpus and produce a ML model \(_languageDescription_\), etc.
* **dataFormat **\(& **dataFormatOther**\): the data format supported by the app/component for the input or output resource; the values are taken from the respective class of the OMTD-SHARE ontology; if none of the suggested values fits the data format, use the broader value and add relevant information in the "dataFormatOther" element
* **language**: the language for the input or output resource of an application/component; the values are taken from the language identifier of the [BCP 47](https://tools.ietf.org/html/bcp47) recommendations

* **annotationType **\(& **annotationTypeOther**\): specifies the annotation type\(s\) of the annotated resource that the application/component takes as input or produces; the values are taken from the respective class of the OMTD-SHARE ontology; if none of the suggested values fits the annotation type of the resource, use the broader value and add relevant information in the "annotationTypeOther" element

**Relation to other metadata schemas**

* processingResourceType
  * UIMA/UIMAfit: Parameters input/output types
* dataFormat
  * **UIMA/UIMA-fit:** @MimeTypeCapability
* language
  * **UIMA/UIMA-fit:** @LanguageTypeCapability
* annotationType

  * **UIMA/UIMA-fit:** @TypeCapability



