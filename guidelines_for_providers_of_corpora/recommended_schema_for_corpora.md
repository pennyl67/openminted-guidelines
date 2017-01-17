## ​Recommended schema for corpora {#recommended-schema-for-corpora}

### Overview {#overview}

This section includes a synopsis of the minimal schema for corpora<sup><sup id="916464963798167-footnote-ref-27"><a href="#916464963798167-footnote-27">[27]</a></sup></sup>, i.e. the subset of M(andatory) and strongly R(ecommended) metadata elements. Additional elements required for the management of the metadata record (e.g. _metadataCreationDate, metadataCreator_ etc.) are not presented here, as they are to be handled by the OMTD platform.

Table 3 - Overview of the recommended OMTD-SHARE schema for corpora

| OMTD-SHARE element | Usage |
| --- | --- |
| resourceType | M |
| resourceName | M |
| description | M |
| identifier | M |
| version | M |
| distributionMedium | M |
| licence or rightsStmtName &amp; rightsStmtURL (one of the two must be provided) | M |
| (licence) version | M |
| distributionMedium | M |
| downloadURL | M when applicable |
| contactEmail or landingPage (one of the two must be provided) | M |
| contactPerson (identifier or personName) | R |
| contactGroup (identifier or organizationName) | R |
| mustBeCitedWith | R |
| resourceCreator | R |
| creationDate | R (M for query built corpora) |
| corpusType | M |
| mediaType | M |
| lingualityType | M |
| multilingualityType | MC |
| language | M |
| size &amp; sizeUnit | M |
| mimeType | R |
| characterEncoding | R |
| domain | R |
| subject | R |
| keyword | R |
| userQuery | M when applicable |
| relationType | R |
| relatedResource1 | R |
| relatedResource2 | R |

### Metadata schema for annotated corpora {#metadata-schema-for-annotated-corpora}

Annotated corpora are documented as separate resources

*   including only the annotated data, with a link to the raw corpus and its own set of metadata elements providing information on the annotation process, tool etc. or
*   as a set of raw and annotated files together, with a metadata record that includes all the appropriate elements for raw corpora (cf. above) with the additional set of metadata elements for annotations, i.e. all the following elements except for &quot;resourceIdentifier&quot;.

Table 4 - Overview of the recommended OMTD-SHARE schema for annotated corpora

| OMTD-SHARE element | Usage |
| --- | --- |
| resourceIdentifier | M |
| annotationLevel | M |
| annotationStandoff | R |
| mimeType | R |
| dataFormatSpecific | R |
| documentationURL | R |
| characterEncoding | R |
| typesystem | R |
| tagset | R |
| annotationMode | R |
| isAnnotatedBy | R |
| annotationDate | R |

[^27]: The full OMTD-SHARE schema is documented at: