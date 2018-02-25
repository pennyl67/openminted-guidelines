## ​Recommended metadata for language descriptions, incl. ML models and grammars {#recommended-schema-for-models}

{% blurb style='tip'%}
You can find more information on the **full OMTD-SHARE metadata schema** and **examples** of metadata records for Language descriptions \(incl. Machine Learning models and computational grammars\)  [here](https://openminted.github.io/releases/omtd-share/3.0.2/).
{% endblurb %}

The following table presents mandatory and recommended elements for Language descriptions \(incl. Machine Learning models and computational grammars\); these have been selected so as to help
* identify the resource and provide information about it \(e.g. resourceIdentifier, resourceName, description\)
* describe the legal terms for using the resource \(e.g. licence or rightsStatement\)
* encode  technical features that are useful for achieving interoperability with TDM tools and services \(e.g. variant, dataFormat, language,  typesystem\)
* give access to the resource \(distributionMedium, distributionLocation\)
* classify the resource along a variety of criteria that end-users can apply for locating resources of interest for their research \(e.g. domain, TDMMethod, algorithm\)
* contribute to attribution, citation and reproducibility of research processes and outputs \(e.g. resourceCreator\).

| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](/models_resourceType.md) | Mandatory |
| [resourceName](/models_resourceName.md) | Mandatory |
| [description](/models_description.md) | Mandatory |
| [resourceIdentifier](/models_identifier.md) | Mandatory |
| [public](/public.md) | Mandatory |
| [version](/version.md) | Mandatory |
| [contactPoint](/contactpoint.md) | Mandatory |
| [contactType](/contacttype.md) | Mandatory |
| [contactPerson](/contactPerson.md) | Recommended |
| [contactGroup](/contactGroup.md) | Recommended |
| [licence](/licence.md) | Mandatory |
| [rightsStatement](/rightsStatement.md) | Mandatory |
| [nonStandardLicenceName](/nonStandardLicenceName.md) and  [nonStandardLicenceTermsURL](/nonStandardLicenceTermsURL.md) | Mandatory when applicable |
| [distributionMedium](/distributionMedium.md) | Mandatory |
| [distributionLocation](/distributionLocation.md) | Mandatory |
| [resourceDocumentationInfo](/resourcedocumentationinfo.md) | Recommended |
| [resourceCreator](/resourceCreator.md) | Recommended |
| [languageDescriptionType](/models_languageDescriptionType.md) | Mandatory |
| [dataFormat](/dataFormat.md) (& dataFormatOther) | Mandatory |
| [variant](/models_variantName.md) | Mandatory |
| [typesystem](/typesystem.md) | Recommended |
| [annotationSchema](/annotationSchema.md) | Recommended when applicable |
| [annotationResource](/annotationResource.md) | Recommended when applicable |
| [TDMMethod](/TDMmethod.md) | Recommended |
| [algorithm](/models_algorithm.md) | Recommended |
| [trainingCorpusDetails](/models_trainingCorpusDetails.md) | Recommended |
| [lingualityType](/models_lingualityType.md) | Mandatory |
| [language](/models_language.md) | Mandatory |
| [size & sizeUnit](/models_size.md) | Recommended |
| [domain](/domain.md) | Recommended |
| [relationType](/relationType.md) | Recommended |
| [relatedResource](/relatedResource.md) | Mandatory when applicable |

