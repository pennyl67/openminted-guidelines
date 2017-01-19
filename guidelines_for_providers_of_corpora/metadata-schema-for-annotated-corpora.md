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

