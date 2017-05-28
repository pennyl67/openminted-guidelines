## ​Recommended schema for ​lexical/conceptual resources, incl. annotation resources {#recommended-schema-for-lexical-conceptual-resources}

The following table presents mandatory and recommended elements for annotation resources; these have been selected so as to help 
* identify the resource and provide information about it: resourceIdentifier, resourceName, version, description, contactPerson, contactEmail, contactGroup, landingPage
* describe the legal terms for using the resource: licence or rightsStatement, nonStandardLicenceName and nonStandardLicenceTermsURL 
* encode  technical features that are useful for achieving interoperability by tools and services: dataFormat, language,  metalanguage, lexicalConceptualResourcetype, mediaType, relationType, relatedResource
* give access to the contents: distributionMedium, distributionURL
* classify the resource along a variety of criteria that end-users can apply for locating resources of interest for their research: contentTypes, domain
* contribute to attribution, citation and reproducibility of experiments: resourceCreator, mustBeCitedWith.


| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](/lcr_resourceType.md) | Mandatory |
| [resourceName](/lcr_resourceName.md) | Mandatory |
| [description](/lcr_description.md) | Mandatory  |
| [resourceIdentifier](/lcr_identifier.md) | Mandatory  |
| [public](/public.md) | Mandatory |
| [version](/version.md) or [versionDate](/versionDate.md) | Mandatory \(choice: one element must be encoded) |
| [licence](/licence.md) or [rightsStatement](/rightsStatement.md) | Mandatory (choice: one of the two must be encoded) |
| [distributionMedium](/lcr_distributionMedium.md) | Mandatory |
| [distributionURL](/distributionURL.md) | Mandatory when applicable |
| [contactPerson](/contactPerson.md) or [contactEmail](/contactEmail.md) or [landingPage](/landingPage.md) | Mandatory (choice: one element must be encoded) |
| [contactGroup](/contactGroup.md) | Recommended |
| [mustBeCitedWith](/mustBeCitedWith.md) | Recommended |
| [lexicalConceptualResourceType](/lcr_lexicalConceptualResourceType.md) | Mandatory |
| [contentTypes](/lcr_contentTypes.md) | Recommended |
| [lingualityType](/lcr_lingualityType.md) | Mandatory |
| [language](/lcr_language.md) | Mandatory |
| [metalanguage](/lcr_metalanguage.md) | Recommended |
| [size](/lcr_size.md) & sizeUnit | Mandatory |
| [dataFormat](/lcr_dataFormat.md) | Recommended |
| [domain](/lcr_domain.md) | Recommended |
| [relationType](/lcr_relationType.md) | Recommended |
| [relatedResource](/lcr_relatedResource.md) | Mandatory when applicable |



