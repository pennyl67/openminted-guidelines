## ​Recommended schema for models {#recommended-schema-for-models}


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
| resourceCreator (person or organization, described with identifier or name) | R |
| variantName | M |
| tagset | R |
| typesystem | R |
| algorithm | R |
| trainingCorpusDetails | R |
| mediaType | M |
| lingualityType | M |
| multilingualityType | M when applicable |
| language | M |
| size and sizeUnit | M |
| collectedFrom : repositoryName or repositoryIdentifier (with attribute) | R |
| sourceMetadataLink | R |
| relationType = isCompatibleWith (external relation between models and components that can use them) | R |