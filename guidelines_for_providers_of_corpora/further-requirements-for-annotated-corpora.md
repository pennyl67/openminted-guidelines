### Further requirements for annotated/processed corpora {#further-requirements-for-annotated-processed-corpora}

Corpora can be registered in the OpenMinTeD platform

* in an unprocessed format \(typical case\) and/or
* in an already processed format.

In the latter case, they must be registered

* as a separate resource 
* with a metadata record including a specific set of [metadata elements](metadata-schema-for-annotated-corpora.md) \(the same as for annotated publications\)
* as a zipped file, which, in addition to the folders of raw corpora \(i.e. "fulltext", "metadata" and "licence"\), will have a folder entitled "annotation" for the annotated files.
* with annotated files encoded in the [XML Metadata Interchange](http://www.omg.org/spec/XMI/) \(XMI\) format, specifically the representation of a [UIMA CAS](https://uima.apache.org/d/uimaj-2.9.0/references.html#ugr.ref.xmi).



