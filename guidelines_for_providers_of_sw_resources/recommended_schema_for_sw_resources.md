### Recommended metadata for software {#recommended-schema-for-s-w-resources}

This section includes a synopsis of the recommended schema for sofware resources, i.e. the subset of Mandatory and strongly Recommended metadata elements, only as regards elements related to the resource itself. Additional elements required for the management of the metadata record \(e.g. _metadataCreationDate, metadataCreator_ etc.\) are not presented here, as they are to be handled by the OMTD platform.

The following table presents mandatory and recommended elements for Machine Learning models; these have been selected so as to help

* identify the resource and provide information about it \(e.g. resourceIdentifier, resourceName, version\)
* describe the legal terms for using the resource \(e.g. licence and rightsStatement\) 
* encode  technical features that are useful for achieving interoperability with content and ancillary knowledge resources \(e.g. application, input and output specifications and dependencies\)
* give access to the component and execute it \(e.g. distributionLocation, command\)
* classify the resource along a variety of criteria that end-users can apply for locating resources of interest for their research \(e.g. function, TDMMethod\)
* contribute to attribution, citation and reproducibility of experiments (e.g. resourceCreator).

| **OMTD-SHARE element** | **Usage** |
| --- | --- |
| [resourceType](/components_resourceType.md) | Mandatory |
| [resourceName](/components_resourceName.md) | Mandatory |
| [description](/components_description.md) | Mandatory |
| [resourceIdentifier](/components_resourceIdentifier.md) | Mandatory |
| [public](/public.md) | Mandatory |
| [version](/version.md) | Mandatory |
| [contactPoint](/contactpoint.md) | Mandatory |
| [contactType](/contacttype.md) | Mandatory |
| [contactPerson](/contactPerson.md) | Recommended |
| [contactGroup](/contactGroup.md) | Recommended |
| [resourceDocumentationInfo](/resourcedocumentationinfo.md) | Recommended |
| [resourceCreator](/resourceCreator.md) | Recommended |
| [application](/components_application.md) | Mandatory |
| [function](/components_function.md) (& functionOther) | Mandatory |
| [componentDistributionForm](/components_componentDistributionForm.md) | Mandatory |
| [distributionLocation](/components_distributionLocation) | Mandatory |
| [command](/components_command.md) | Mandatory when applicable |
| [licence](/licence.md) | Mandatory |
| [rightsStatement](/rightsStatement.md) | Mandatory |
| [nonStandardLicenceName](/nonStandardLicenceName.md) and  [nonStandardLicenceTermsURL](/nonStandardLicenceTermsURL.md) | Mandatory when applicable |
| [parameterInfo](/parameterinfo.md) | Mandatory when applicable |
| [inputContentResourceInfo](/inputcontentresourceinfo.md) | Mandatory when applicable |
| [outputResourceInfo](/outputresourceinfo.md) | Mandatory when applicable |
| [previousAnnotationTypesPolicy](/previousannotationtypespolicy.md) | Mandatory when applicable |
| [componentDependencies](/componentdependencies.md) | Mandatory when applicable |
| [framework](/components_framework.md) | Mandatory |
| [TDMMethod](/TDMmethod.md) | Recommended |
| [relationType](/relationType.md) | Recommended |
| [relatedResource](/relatedResource.md) | Mandatory when applicable |



