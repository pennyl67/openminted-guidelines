## ​Recommended metadata for corpora {#recommended-schema-for-corpora}

This section includes a synopsis of the minimal schema for corpora, i.e. the subset of Mandatory and strongly Recommended metadata elements. Additional elements required for the management of metadata record \(e.g. _metadataCreationDate, metadataCreator_ etc.\) are not presented here, as they are to be handled by the OpenMinTeD platform.

These elements have been selected so as to help

* identify the corpus and provide information about it \(e.g. resourceIdentifier, resourceName, version, description\)
* describe the legal terms for using the corpus \(e.g. licence or rightsStatement, nonStandardLicenceTermsURL\)
* encode  technical features that are useful for achieving interoperability by tools and services \(e.g. dataFormat, language\)
* give access to the contents \(e.g. distributionLocation\)
* classify the corpus along a variety of criteria that end-users can apply for locating corpora of interest for their research \(e.g. domain, keyword\)
* contribute to attribution, citation and reproducibility of research processes and outputs: \(e.g. resourceCreator, creationDate, userQuery\).

For annotated corpora, see [here](metadata-schema-for-annotated-corpora.md).

| **OMTD-SHARE element** | **Usage** |
| --- | --- |
| [resourceType](/corpora_resourceType.md) | Μandatory |
| [resourceName](/corpora_resourceName.md) | Μandatory |
| [description](/corpora_description.md) | Μandatory |
| [resourceIdentifier](/corpora_identifier.md) | Μandatory |
| [public](/public.md) | Mandatory |
| [contactEmail](/contactEmail.md) or [landingPage](/landingPage.md) or [contactPerson](/contactPerson.md) | Μandatory  \(choice:one element must be encoded\) |
| [contactGroup](/contactGroup.md) | Recommended |
| [version](/version.md) or [versionDate](/versionDate.md) | Mandatory \(choice: one element must be encoded\) |
| [licence](/licence.md) or [rightsStatement](/rightsStatement.md) | Mandatory \(choice: one element must be encoded\) |
| [nonStandardLicenceName](/nonStandardLicenceName.md) and [nonStandardLicenceTermsURL](/nonStandardLicenceTermsURL.md) | Mandatory upon conditions |
| [distributionMedium](/corpora_distributionMedium.md) | Μandatory |
| [distributionURL](/distributionURL.md) | Μandatory when applicable |
| [mustBeCitedWith](/mustBeCitedWith.md) | Recommended |
| [resourceCreator](/resourceCreator.md) | Recommended |
| [creationDate](/corpora_creationDate.md) | Recommended \(Mandatory for query- built corpora\) |
| [corpusSubtype](/corpora_corpusSubtype.md) | Μandatory |
| [mediaType](/corpora_mediaType.md) | Μandatory |
| [lingualityType](/corpora_lingualityType.md) | Μandatory |
| [multilingualityType](/corpora_multilingualityType.md) | Μandatory when applicable |
| [language](/corpora_language.md) | Μandatory |
| [size](/corpora_size.md) | Μandatory |
| [dataFormat](/corpora_dataFormat.md) | Recommended |
| [domain](/corpora_domain.md) | Recommended |
| [keyword](/corpora_keyword.md) | Recommended |
| [userQuery](/corpora_userQuery.md) | Μandatory when applicable |
| [relationType](/corpora_relationType.md) | Recommended |
| [relatedResource](/corpora_relatedResource.md) | Recommended |



