## ​Recommended metadata for ML models {#recommended-schema-for-models}
The following table presents mandatory and recommended elements for Machine Learning models; these have been selected so as to help 
* identify the resource and provide information about it: resourceIdentifier, resourceName, version, description, contactPerson, contactEmail, contactGroup, landingPage
* describe the legal terms for using the resource: licence or rightsStatement, nonStandardLicenceName and nonStandardLicenceTermsURL 
* encode  technical features that are useful for achieving interoperability with TDM tools and services: variant, dataFormat, language,  typesystem, annotationSchema, annotationResource, relationType, relatedResource
* give access to the resource: distributionMedium, distributionURL, command
* classify the resource along a variety of criteria that end-users can apply for locating resources of interest for their research: domain, TDMMethod, algorithm
* contribute to attribution, citation and reproducibility of experiments: resourceCreator, mustBeCitedWith.

| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](/models_resourceType.md) | Mandatory |
| [resourceName](/models_resourceName.md) | Mandatory |
| [description](/models_description.md) | Mandatory  |
| [resourceIdentifier](/models_identifier.md) | Mandatory |
| [public](/public.md) | Mandatory |
| [version](/version.md) | Mandatory |
| [licence](/licence.md) or [rightsStatement](/rightsStatement.md)  | Mandatory (choice: one element must be encoded) |
| [distributionMedium](/models_distributionMedium.md) | Mandatory |
| [distributionURL](/distributionURL.md) | Mandatory when applicable |
| [contactPerson](/contactPerson.md) or [contactEmail](/contactEmail.md) or [landingPage](/landingPage.md) | Mandatory (choice: one element must be encoded) |
| [contactGroup](/models_contactGroup.md) | Recommended |
| [mustBeCitedWith](/mustBeCitedWith.md) | Recommended |
| [resourceCreator](/resourceCreator.md) | Recommended |
| [languageDescriptionType](/models_languageDescriptionType.md) | Mandatory |
| [variant](/models_variantName.md) | Mandatory |
| [typesystem](/annotations_typesystem.md) | Recommended |
| [annotationSchema](/annotations_annotationSchema.md) | Recommended when applicable |
| [annotationResource](/annotations_annotationResource.md) | Recommended |
| [TDMMethod](/TDMmethod.md) | Recommended |
| [algorithm](/models_algorithm.md) | Recommended |
| [trainingCorpusDetails](/models_trainingCorpusDetails.md) | Recommended |
| [mediaType](/models_mediaType.md) | Mandatory |
| [lingualityType](/models_lingualityType.md) | Mandatory |
| [language](/models_language.md) | Mandatory |
| [size & sizeUnit](/models_size.md) | Recommended |
| [relationType](/models_relationType.md)  | Recommended |
| [relatedResource](/models_relatedResource.md)  | Mandatory when applicable |
