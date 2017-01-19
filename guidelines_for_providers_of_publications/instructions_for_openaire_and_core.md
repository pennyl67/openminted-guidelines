## ​Instructions for OpenAIRE and CORE {#instructions-for-openaire-and-core}

OpenAIRE and CORE will bring content resources into OpenMinTeD through user queries.

End-users that wish to run TDM services on specific content will be presented with a faceted view of the OpenAIRE and CORE contents; by selecting from a range of criteria, a query will gradually be built which will be transferred to the respective APIs and retrieve the metadata records and data files of the matching publications. It should be noted that

****only publications that provide the full text or, at least, an abstract are candidate for inclusion in OpenMinTeD.****

For each new corpus created according to this procedure, an automatically generated metadata record will be produced which will be submitted to the user for further editing.

### Packaging and uploading instructions {#packaging-and-uploading-instructions}

The transfer layer between OpenAIRE/CORE and the OMTD platform will make use of **RESTful calls**.

The delivery of the requested publications must be made in a compressed file, with the following folder structure:

*   one folder with all the metadata records entitled &quot;metadata records&quot;
*   one folder with all the publications contents entitled &quot;files&quot;
*   one folder with all the licence documents provided with the material entitled &quot;licences&quot;.

### Documentation/​Metadata requirements {#documentation-metadata-requirements}

In the case of publications, the required metadata records come at two levels:

*   one for the whole query-generated corpus of publications, in compliance with the OMTD-SHARE schema for corpora, which is automatically constructed on the basis of the user filters and manually enriched by the user;
*   one per publication, with a minimal set of metadata elements in compliance with the OMTD-SHARE schema for publications, automatically converted from the current schemas of the providers.

It should be noted that the resource providers do not have to change their current schemas<sup id="916464963798167-footnote-ref-16"><a href="#916464963798167-footnote-1">[1]</a></sup>; mappings and conversions between OpenAIRE/CORE and the OMTD-SHARE schema are made in the framework of OpenMinTeD

All metadata records for publications must be delivered in XML format.

### Further requirements for annotated/processed publications {#further-requirements-for-annotated-processed-publications}

Scholarly publications will normally be imported into the OpenMinTeD platform in an unprocessed format and will be annotated by the operation of TDM software also registered in the platform. However, certain providers may decide to run the TDM or annotation software at their own premises and upload the results of the processing directly into OpenMinTeD (e.g. annotating the publications with structural markup, extracting acknowledgements or citations sections etc.).

In these cases, the annotated output is considered a new resource and, therefore, should be uploaded

*   as a separate resource from the raw publication in a folder called &quot;annotated files&quot;
*   with its own metadata record, following the instructions for annotated publications.

It should be noted that publications annotated by means of the OpenMinTeD platform will be automatically assigned the appropriate values for these elements.

[^1]: The OpenAIRE schema and guidelines are currently under revision; collaboration with the relevant actors has been established to take into account the new features and, where desired, influence the changes so as to support TDM processes in accordance to the interoperability requirements.
