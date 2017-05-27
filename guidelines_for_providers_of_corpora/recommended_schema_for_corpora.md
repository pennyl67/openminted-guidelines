## ​Recommended metadata for corpora {#recommended-schema-for-corpora}

This section includes a synopsis of the minimal schema for corpora, i.e. the subset of Mandatory and strongly Recommended metadata elements. Additional elements required for the management of metadata record (e.g. _metadataCreationDate, metadataCreator_ etc.) are not presented here, as they are to be handled by the OpenMinTeD platform.

These elements have been selected so as to help 
* identify the corpus and provide information about it: resourceIdentifier, resourceName, version, description, contactPerson, contactEmail, contactGroup, landingPage
* describe the legal terms for using the corpus: licence or rightsStatement, nonStandardLicenceName and nonStandardLicenceTermsURL 
* encode  technical features that are useful for achieving interoperability by tools and services: dataFormat, language, characterEncoding, corpusSubtype, mediaType, relationType, relatedResource
* give access to the contents: distributionMedium, distributionURL
* classify the corpus along a variety of criteria that end-users can apply for locating corpora of interest for their research: domain, keyword
* contribute to attribution, citation and reproducibility of experiments: resourceCreator, creationDate, userQuery, mustBeCitedWith.

For annotated corpora, see [here](metadata-schema-for-annotated-corpora.md).

| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](/corpora_resourceType.md) | Μandatory |
| [resourceName](/corpora_resourceName.md) | Μandatory |
| [description](/corpora_description.md) | Μandatory |
| [resourceIdentifier](/corpora_identifier.md) | Μandatory |
| [public](/corpora_public.md) | Mandatory |
| [contactEmail](/corpora_contactEmail.md) or [landingPage](/corpora_landingPage.md) or [contactPerson](/corpora_contactPerson.md)  | Μandatory  \(choice:one element must be encoded) |
| [contactGroup](/corpora_contactGroup.md) | Recommended |
| [version](/corpora_version.md) or [versionDate](/corpora_versionDate.md) | Mandatory \(choice:one element must be encoded) |
| [licence](/corpora_licence.md) or [rightsStatement](/corpora_rightsStatement.md) | Mandatory (choice: one element must be encoded) |
| [nonStandardLicenceName](/corpora_nonStandardLicenceName.md) and [nonStandardLicenceTermsURL](/corpora_nonStandardLicenceTermsURL.md) | Mandatory upon conditions |
| [distributionMedium](/corpora_distributionMedium.md) | Μandatory |
| [distributionURL](/corpora_distributionURL.md) | Μandatory when applicable |
| [mustBeCitedWith](/corpora_mustBeCitedWith.md) | atoryRecommended |
| [resourceCreator](/corpora_resourceCreator.md) | Recommended |
| [creationDate](/corpora_creationDate.md) | Recommended \(Mandatory for query- built corpora\) |
| [corpusSubtype](/corpora_corpusSubtype.md) | Μandatory |
| [mediaType](/corpora_mediaType.md) | Μandatory |
| [lingualityType](/corpora_lingualityType.md) | Μandatory |
| [multilingualityType](/corpora_multilingualityType.md) | Μandatory when applicable |
| [language](/corpora_language.md) | Μandatory |
| [size](/corpora_size.md) | Μandatory |
| [dataFormat](/corpora_dataFormat.md) | Recommended |
| [characterEncoding](/corpora_characterEncoding.md) | Recommended |
| [domain](/corpora_domain.md) | Recommended |
| [keyword](/corpora_keyword.md) | Recommended |
| [userQuery](/corpora_userQuery.md) | Μandatory when applicable |
| [relationType](/corpora_relationType.md) | Recommended |
| [relatedResource](/corpora_relatedResource.md) | Recommended |
