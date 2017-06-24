#### dataFormat
##### Usage
Recommended
##### Type
open controlled vocabulary
##### Controlled vocabulary reference and/or values
ms:dataFormat (a subset of values (the most popular ones for text files) from the IANA mimetype controlled vocabulary and more specific dataFormats): _text/plain_, _application/vnd.xmi+xml_, _application/xml_, _application/x-xces+xml_, _application/tei+xml_, _application/rdf+xml_, _application/xhtml+xml_, _application/emma+xml_, _application/pls+xml_, _application/postscript_, sgml_, _text/html_, _application/x-tex_, _application/rtf_, _application/json+ld_, _application/x-latex_, _text/csv_, _text/tab-separated-values_, _application/pdf_, _application/x-msaccess_, _application/msword_, _application/vnd.ms-excel_,  _text/turtle_, _other_, 
_aclAnthology_, _aimedCorpus_, _ alvisEnrichedDocument_, _bioNLP_, _ bioNLP; format-variant=ST2013a1_a2_, _bnc_, _cadixeJSON_, _conll2000_, _conll2002_, _conll2006_, _conll2007_, _conll2009_, _conll2012_, _dataSift_, _factoredTagLem_, _gate_, _genia_, _graf_, _html5Microdata_, _i2b2_, _imsCwb_, _jdbc_, _keaCorpus_, _lll_, _negraExport_, _pml_, _ptb; format-variant=chunked_, _ptb; format-variant=combined_, _relp_, _tiger_, _tupp-dz_, _twitter_, _uimaBinaryCas_, _uimaCASDump_, _web1t_, _xces; format-variant=ilsp_
##### Definition/Explanations
Specifies the format that is used since often the mime type will not be sufficient for machine processing.
NOTE: normally the format should be represented as a combination of the mimetype (e.g. application/xml) and some name and link to the documentation about the supplementary conventions used (e.g xces, alvisED etc.)
##### Recommended usage
Please, use to specify the format of the resource supported by the component (as input or output). 
For interoperability reasons, it is important to standardise as far as possible this element; this is why a list of values including the formats currently supported by components in the OpenMinTeD registry is provided. Where possible, it is also recommended to use the "documentationURL" element with information and examples about the specific data format.
