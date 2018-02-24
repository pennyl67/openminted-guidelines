### Further requirements for annotated publications {#further-requirements-for-annotated-publications}

Scholarly publications will normally be imported into the [OpenMinTeD platform](https:\\services.openminted.eu) in an unprocessed format and will be annotated by the operation of TDM software also registered in the platform.

However, certain providers may decide to run the TDM or annotation software at their own premises and upload the results of the processing directly into OpenMinTeD \(e.g. annotating the publications with structural markup, recognizing acknowledgements or citations sections etc.\).

{% blurb style='warning'%}
The mechanism for using as input of a TDM application annotated publications is under construction in the OpenMinTeD platform.
{% endblurb %}

In these cases, the annotated output (publication) is considered a new resource and should follow the technical specifications that have been set for processing resources inside the OpenMinTeD platform. More specifically, it should be
* encoded with the [XML Metadata Interchange](http://www.omg.org/spec/XMI/) \(XMI\) format, and most specifically with a [UIMA CAS](https://uima.apache.org/d/uimaj-2.9.0/references.html#ugr.ref.xmi)
* described with its own metadata record, using [metadata for annotated publications](/guidelines_for_providers_of_publications/metadata-schema-for-annotated-publications.md)
* packaged with all other raw and annotated publications into a corpus and registered following the instructions for [sharing corpora](/guidelines_for_providers_of_corpora/instructions_for_providers_of_corpora.md).


