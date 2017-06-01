### Further requirements for annotated/processed corpora {#further-requirements-for-annotated-processed-corpora}

Corpora can be registered in the OpenMinTeD platform

* in an unprocessed format and annotated by the operation of TDM software also registered in the platform and/or
* in an already processed format; in this case, they must be included as a separate resource with a specific metadata record including a specific set of [metadata elements](metadata-schema-for-annotated-corpora.md) \(the same as for annotated publications\).

It should be noted that corpora annotated by means of the OpenMinTeD platform will be automatically assigned the appropriate values for these elements.

As regard the data format of annotated corpora, please note that OpenMinTeD has endorsed the use of the [XML Metadata Interchange](http://www.omg.org/spec/XMI/) \(XMI\) format, specifically the representation of a [UIMA CAS](https://uima.apache.org/d/uimaj-2.9.0/references.html#ugr.ref.xmi) to encode annotations on text in particular when exchanging data between components within a workflow; the RDF-based [WebAnnotation](https://www.w3.org/annotation/) standard will be used to make annotations produced by OpenMinTeD workflows accessible to third parties and to encode annotations above the text level, e.g. on document/collection level.



