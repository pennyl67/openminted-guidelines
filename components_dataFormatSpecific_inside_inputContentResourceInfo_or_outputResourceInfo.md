#### dataFormatSpecific inside inputContentResourceInfo or outputResourceInfo
##### Usage
Mandatory when applicable
##### Conditions for usage
if the input content resource (i.e. the resource to be mined) or the output resource (the results of the processing) is to be described, this element is obligatory
##### Type
open controlled vocabulary
##### Controlled vocabulary reference and/or values
aclAnthology aimedCorpus alvisEnrichedDocument bioNLP bioNLP; format-variant=ST2013a1_a2bnc cadixeJSON conll2000 conll2002 conll2006 conll2007 conll2009 conll2012 dataSift factoredTagLem gate genia graf html5Microdata i2b2 imsCwb jdbc keaCorpus lll negraExport pml ptb; format-variant=chunked ptb; format-variant=combined relp tiger tupp-dz twitter uimaBinaryCas uimaCASDump web1t xces; format-variant=ilsp: 
##### Definition/Explanations
The supplementary level of data format
##### Recommended usage
Please, use to further specify the format of the resource supported by the component (as input or output). 
For interoperability reasons, it is important to standardise as far as possible this element; this is why a list of values including the formats currently supported by components in the OMTD registry is provided. Where possible, it is also recommended to use the "documentationURL" element with information and examples about the specific data format.
##### Relation to other metadata schemas
* **UIMA/UIMA-fit:** @MimeTypeCapability
