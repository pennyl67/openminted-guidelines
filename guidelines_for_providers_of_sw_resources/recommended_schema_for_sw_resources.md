## Recommended schema for s/w resources {#recommended-schema-for-s-w-resources}

This section includes a synopsis of the recommended schema for s/w resources, i.e. the subset of M(andatory) and strongly R(ecommended) metadata elements, only as regards elements related to the resource itself. Additional elements required for the management of the metadata record (e.g. _metadataCreationDate, metadataCreator_ etc.) are not presented here, as they are to be handled by the OMTD platform.

| OMTD-SHARE element | Usage |
| --- | --- |
| resourceType | M |
| resourceName | M |
| description | M |
| identifier | M |
| version | M |
| componentDistributionMedium | M |
| componentType | M |
| licence or rightsStmtName &amp; rightsStmtURL (one of the two must be provided) | M |
| (licence) version | M |
| contactEmail or landingPage (one of the two must be provided) | M |
| contactPerson (identifier or personName) | R |
| contactGroup (identifier or organizationName) | R |
| mailingList (mailingListName, subscribe, unsubscribe, post, archive, otherArchive) | R |
| issueTracker | R |
| onlineHelpURL | R |
| mustBeCitedWith | R |
| downloadURL or accessURL (one of the two should be provided) | M when applicable |
| resourceCreator (person or organization, described with identifier or name) | R |
| inputContentResourceInfo or outputContentResourceInfo/mediaType (i.e. mediaType of input and output resource) | M when applicable |
| inputContentResourceInfo or outputContentResourceInfo/resourceType | R when applicable |
| inputContentResourceInfo or outputContentResourceInfo/language | R when applicable |
| inputContentResourceInfo or outputContentResourceInfo/characterEncoding | R when applicable |
| inputContentResourceInfo or outputContentResourceInfo/mimeType | R when applicable |
| inputContentResourceInfo or outputContentResourceInfo/dataFormatSpecific | R when applicable |
| inputContentResourceInfo or outputContentResourceInfo/typesystem | R when applicable |
| inputContentResourceInfo or outputContentResourceInfo/tagset | R when applicable |
| inputContentResourceInfo or outputContentResourceInfo/annotationLevel | R when applicable |
| typesystem | R |
| tagset | R |
| annotationResource | R |
| framework | R |
| for parameters: parameterName, description, parameterType, mandatory, multiValue | M when applicable |
| collectedFrom : repositoryName or repositoryIdentifier (with attribute) | R |
| sourceMetadataLink | R |
| relationType=isCompatibleWith (external relation; link to models, annotation resources etc. that can be used with the component) | R |

[^42]: The full OMTD-SHARE schema is documented at: