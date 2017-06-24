### Further requirements for annotated publications {#further-requirements-for-annotated-publications}

Scholarly publications will normally be imported into the OpenMinTeD platform in an unprocessed format and will be annotated by the operation of TDM software also registered in the platform.

However, certain providers may decide to run the TDM or annotation software at their own premises and upload the results of the processing directly into OpenMinTeD \(e.g. annotating the publications with structural markup, extracting acknowledgements or citations sections etc.\).

In these cases, the annotated output is considered a new resource and, therefore, should be registered

* as a separate resource from the raw publication in a folder called "annotated files"
* with its own metadata record, following the [instructions for annotated publications](/guidelines_for_providers_of_publications/metadata-schema-for-annotated-publications.md).

It should be noted that publications annotated by means of the OpenMinTeD platform will be automatically assigned the appropriate values for these elements.

As regard the data format of annotated publications, please note that OpenMinTeD has endorsed the use of the [XML Metadata Interchange](http://www.omg.org/spec/XMI/) \(XMI\) format, specifically the representation of a [UIMA CAS](https://uima.apache.org/d/uimaj-2.9.0/references.html#ugr.ref.xmi) to encode annotations on text in particular when exchanging data between components within a workflow; the  [WebAnnotation](https://www.w3.org/annotation/) standard will be used to make annotations produced by OpenMinTeD workflows accessible to third parties and to encode annotations above the text level, e.g. on document/collection level.



