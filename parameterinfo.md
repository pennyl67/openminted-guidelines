#### parameterInfo

##### Usage

Mandatory when applicable

**Type**

set of elements

**Mandatory and recommended elements**

| **Element** | **Usage** | **Type** |
| :--- | :--- | :--- |
| parameterName | Mandatory | free text |
| parameterLabel | Mandatory | free text |
| parameterDescription | Mandatory | free text |
| parameterType | Mandatory | controlled vocabulary |
| optional | Mandatory | boolean |
| multiValue | Mandatory | boolean |
| defaultValue | Mandatory when applicable | free text |
| dataFormat \(& dataFormatOther\) | Mandatory when applicable | open controlled vocabulary |

##### Definition/Explanations

Groups together information on each parameter of an application or component.

* **parameterName**: a name used to identify the parameter
* **parameterLabel**: a label used to show the user for a parameter
* **parameterDescription**: provides a short account of the parameter \(function it performs, input / output requirements etc.\) in free text
* **parameterType**: Classifies the parameter according to a specific \(not yet standardised\) typing system \(e.g. whether it's boolean, string, integer, a document, mapping etc.\)
* **optional**: Specifies whether the parameter is mandatory or optional; the default value is set to true
* **multiValue**: Specifies whether the parameter takes a list of values; the default value is set to false
* **dataFormat **\(& **dataFormatOther**\): the data format supported by the app/component for the input or output resource; the values are taken from the respective class of the OMTD-SHARE ontology; if none of the suggested values fits the data format, use the broader value and add relevant information in the "dataFormatOther" element



