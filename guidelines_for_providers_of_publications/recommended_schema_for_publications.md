## ​Recommended schema for publications {#recommended-schema-for-publications}

### Overview {#overview}

This section includes the overview of the recommended OMTD-SHARE schema<sup><sup id="916464963798167-footnote-ref-18"><a href="#916464963798167-footnote-18">[18]</a></sup></sup> for publications, i.e. the subset of M(andatory) and strongly R(ecommended) metadata elements, only as regards elements related to the resource itself. Additional elements required for the management of the metadata record (e.g. _metadataCreationDate, metadataCreator_ etc.) are not presented here, as they are to be handled by the OMTD platform.

Table 2- Overview of the recommended OMTD-SHARE schema for publications

| OMTD-SHARE element | Usage |
| --- | --- |
| documentType | M |
| publicationType | M |
| identifier | M |
| title | M |
| distributionMedium | M |
| licence or [rightsStmtName &amp; rightsStmtURL] (one of the two must be provided) | M |
| (licence) version | Μ |
| downloadURL | Μ when applicable |
| fullText | R |
| abstract | R |
| author | R |
| publisher | R |
| journal | R |
| mimeType | R |
| characterEncoding | R |
| publicationDate | R |
| subject | R |
| keyword | R |
| collectedFrom: repositoryName or repositoryIdentifier | R |
| sourceMetadataLink | R |
| originalDataProviderType | R |
| originalDataProviderRepository | R when applicable |
| originalDataProviderJournal | R when applicable |
| originalDataProviderPublisher | R when applicable |
| relationType | R |
| relatedResource1 | R |
| relatedResource2 |  |

### Metadata schema for annotated publications {#metadata-schema-for-annotated-publications}

Annotated publications are documented as separate resources with a link to the raw publication and their own set of metadata elements providing information on the annotation process, tool etc.

Table 2- Overview of the recommended OMTD-SHARE schema for annotated publications

| OMTD-SHARE element | Usage |
| --- | --- |
| publicationIdentifier | M |
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

[^18]: The full OMTD-SHARE schema is documented at: