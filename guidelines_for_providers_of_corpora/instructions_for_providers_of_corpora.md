## Instructions for providers of corpora {#instructions-for-providers-of-corpora}

### Packaging and uploading instructions {#packaging-and-uploading-instructions}

Corpora can be uploaded by registered users as decided in the OpenMinTeD Policies.

If you wish to share a corpus, you must:

*   provide a metadata record compliant with the OMTD-SHARE schema for corpora, at least at the minimal level which you can upload to the Registry as an XML file and/or edit with the OpenMinTeD metadata editor
*   provide a zipped file with the contents of the corpus or a link to a URL where the corpus is directly accessible (i.e. not a landing page); where possible, the zipped file should follow the folder structure recommended for OpenMinTeD publications, i.e. separate folders for contents, metadata records and licence documents.

If the corpus is stored at the repository of a network or infrastructure that allows harvesting (normally upon agreements made with OpenMinTeD), you can also provide the relevant identifier and this will be uploaded with the appropriate description. Where possible (and this will be appropriately indicated), the metadata description will be automatically converted to the OMTD-SHARE schema and presented to the user for further editing.

### Technical requirements {#technical-requirements}

There are no general requirements yet for corpora to be used for ancillary purposes, as these are dependent on the requirements of the s/w components that will use them and on the purpose of use.

For corpora that will be used for TDM, the requirements are the same with the ones set for corpora produced automatically through user queries in the OpenMinTeD platform to the extent possible - repeated hereafter. For legacy corpora, especially, not all requirements and recommendations can be enforced, but for new corpora, the adoption of standards, best practices and recommendations promoted by OpenMinTeD and other infrastructures should be taken into account from the early steps of design and specifications.

Please, note that the list below is meant to provide recommendations that contribute to interoperability; if you fail to abide to them, it might still be possible to process your corpora via the OpenMinTeD platform, but this cannot be guaranteed and interoperability with other resources will suffer loss.

*   The preferred formats for delivering textual material are plain txt, xml, pdf (not proprietary and certainly not of scanned images), which can be read by one of the existing readers.
*   If appropriate for your material, use one of the more specific data formats that are already covered by readers and converters (pending link)
*   The preferred character encoding is UTF-8.

### Documentation/Metadata requirements {#documentation-metadata-requirements}

To be fully compliant with OpenMinTeD, you must

*   ensure that the corpus is distributed under Open Access conditions
*   include in the metadata record a link to the licence document that describes the terms and conditions under which it is provided, and attach the licence document together with the resource
*   if you already have a PID for your publication (preferably DOI), make sure it is included in the metadata record.

****Further recommendations will contribute to the interoperability of your resources:****

*   Further adoption of standards such as the JATS article tag suite<sup><sup id="916464963798167-footnote-ref-20"><a href="#916464963798167-footnote-20">[20]</a></sup></sup> or TEI P5 guidelines[^21] for annotating the inner structure of texts is recommended.
*   Please, ensure that you version all your resources and label the versions in an unambiguous way, preferably following the Semantic Versioning recommendations[^22].
*   It is important that you provide the appropriate documentation for your resource (e.g. publications about the design and construction of the corpus etc.), which you should also version along with the corpus and add as reference to your metadata record.
*   Recommend one of the publications about your resource as the one to be cited for scholarly attribution and add this information in the metadata record.
*   Make sure that you fill in the metadata record all the elements required for citing your resource<sup><sup id="916464963798167-footnote-ref-23"><a href="#916464963798167-footnote-23">[23]</a></sup></sup>, i.e. the creator of the resource, a title, the resource type and an identifier, and optionally, the publication date, the version and the publisher or distributor of
*   Use standard classification vocabularies (e.g. MeSH<sup><sup id="916464963798167-footnote-ref-24"><a href="#916464963798167-footnote-24">[24]</a></sup></sup>, DDC<sup><sup id="916464963798167-footnote-ref-25"><a href="#916464963798167-footnote-25">[25]</a></sup></sup>, LCSH<sup><sup id="916464963798167-footnote-ref-26"><a href="#916464963798167-footnote-26">[26]</a></sup></sup> etc.) for adding classification tags to your material and specify the vocabulary you use in the metadata record; give at least one broad category for your material (e.g. life sciences, computing etc.).
*   In all cases, where linking to other resources or entities (e.g. persons, projects etc.) in the metadata records is added, please try to do this through unique and persistent identifiers of authority lists and sources, to the extent possible, documenting also the authority and/or scheme it adheres to.

### Further requirements for annotated/processed corpora {#further-requirements-for-annotated-processed-corpora}

Corpora can be registered in the OpenMinTeD platform

*   in an unprocessed format and annotated by the operation of TDM software also registered in the platform and/or
*   in an already processed format; in this case, they must be included as a separate resource with its own metadata record including a specific set of metadata elements (the same as for annotated publications).

It should be noted that corpora annotated by means of the OpenMinTeD platform will be automatically assigned the appropriate values for these elements.

[^20]: https://jats.nlm.nih.gov/index.html

[^21]: http://www.tei-c.org/Guidelines/P5/

[^22]: 

[^23]: For citation, OpenMinTeD endorses the

[^24]: Medical Subject Headings (https://www.nlm.nih.gov/mesh/)

[^25]: Dewey Decimal Classification (https://www.oclc.org/dewey.en.html)

[^26]: Library of Congress Subject Headings (http://id.loc.gov/authorities/subjects.html)