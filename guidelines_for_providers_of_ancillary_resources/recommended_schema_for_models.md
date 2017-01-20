## ​Recommended schema for models {#recommended-schema-for-models}


| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](\models_resourceType.md) | M  |
| [resourceName](\models_resourceName.md) | M  |
| [description](\models_description.md) | M  |
| [identifier](\models_identifier.md) | M  |
| [version](\models_version.md) | M  |
| [distributionMedium](\models_distributionMedium.md) | M  |
| [licence](\models_licence.md) or [rightsStmtName](\models_rightsStmtName.md) &amp; [rightsStmtURL](\models_rightsStmtURL.md) \(one of the two must be provided\)  | M  |
| [version of licence](\models_version_of_licence|.md) | M  |
| [distributionMedium](\models_distributionMedium.md) | M  |
| [downloadURL](\models_downloadURL.md) | M when applicable  |
| [contactEmail](\models_contactEmail.md) or [landingPage](\models_landingPage.md) \(one of the two must be provided\) | M  |
| [contactPerson](\models_contactPerson.md) \(identifier or personName\) | R  |
| [contactGroup](\models_contactGroup.md) \(identifier or organizationName\) | R  |
| [mustBeCitedWith](\models_mustBeCitedWith.md) | R  |
| [resourceCreator](\models_resourceCreator.md) \(person or organization, described with identifier or name\) | R  |
| [variantName](\models_variantName.md) | M  |
| [tagset](\models_tagset.md) | R  |
| [typesystem](\models_typesystem.md) | R  |
| [algorithm](\models_algorithm.md) | R  |
| [trainingCorpusDetails](\models_trainingCorpusDetails.md) | R  |
| [mediaType](\models_mediaType.md) | M  |
| [lingualityType](\models_lingualityType.md) | M  |
| [multilingualityType](\models_multilingualityType.md) | M when applicable  |
| [language](\models_language.md) | M  |
| [size](\models_size.md) | M  |
| [relationType](\models_relationType.md) = isCompatibleWith (external relation between models and components that can use them)](\models_relationType = isCompatibleWith (external relation between models and components that can use them).md) | R  |
| relationType = isCompatibleWith (external relation between models and components that can use them) | R |