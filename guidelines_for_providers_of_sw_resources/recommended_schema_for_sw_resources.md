### Recommended metadata for software {#recommended-schema-for-s-w-resources}

This section includes a synopsis of the recommended schema for sofware resources, i.e. the subset of Mandatory and strongly Recommended metadata elements, only as regards elements related to the resource itself. Additional elements required for the management of the metadata record \(e.g. _metadataCreationDate, metadataCreator_ etc.\) are not presented here, as they are to be handled by the OMTD platform.

The following table presents mandatory and recommended elements for Machine Learning models; these have been selected so as to help

* identify the resource and provide information about it \(e.g. resourceIdentifier, resourceName, version\)
* describe the legal terms for using the resource \(e.g. licence or rightsStatement\) 
* encode  technical features that are useful for achieving interoperability with content and ancillary knowledge resources \(e.g. componentType, application, input and output specifications and dependencies\)
* give access to the component and execute it \(e.g. distributionLocation, command\)
* classify the resource along a variety of criteria that end-users can apply for locating resources of interest for their research 
  \(e.g. function, TDMMethod\)
* contribute to attribution, citation and reproducibility of experiments \(e.g. resourceCreator, mustBeCitedWith\).

| **OMTD-SHARE element** | **Usage** |
| --- | --- |
| [resourceType](/components_resourceType.md) | Mandatory |
| [resourceName](/components_resourceName.md) | Mandatory |
| [description](/components_description.md) | Mandatory |
| [resourceIdentifier](/components_identifier.md) | Mandatory |
| [public](/components_public.md) | Mandatory |
| [version](/components_version.md) | Mandatory |
| [contactPoint](/contactpoint.md) | Mandatory |
| [contactType](/contacttype.md) | Mandatory |
| [contactPerson](/components_contactPerson.md) | Recommended |
| [contactGroup](/components_contactGroup.md) | Recommended |
| [resourceDocumentationInfo](/resourcedocumentationinfo.md) | Recommended |
| [application](/components_application.md) | Mandatory |
| [function](/components_componentType.md) | Mandatory |
| [functionOther](/functionother.md) | Mandatory when applicable |
| [componentDistributionForm](/components_componentDistributionForm.md) | Mandatory |
| [distributionLocation](/components_downloadURL) | Mandatory |
| [command](/components_command.md) | Mandatory upon conditions |
| [licence](/components_licence.md) | Mandatory |
| [rightsStatement](//rightsStatement.md) | Mandatory |
| [nonStandardLicenceName](/components_nonStandardLicenceName.md) and  [nonStandardLicenceTermsURL](/components_nonStandardLicenceTermsURL.md) | Mandatory upon conditions |
| [parameterInfo](/parameterinfo.md) | Mandatory when applicable |
| [inputContentResourceInfo](/inputcontentresourceinfo.md) | Mandatory when applicable |
| [outputResourceInfo](/outputresourceinfo.md) | Mandatory when applicable |
| [previousAnnotationTypesPolicy](/previousannotationtypespolicy.md) | Mandatory when applicable |
| [componentDependencies](/componentdependencies.md) | Mandatory when applicable |
| [framework](/components_framework.md) | Mandatory |
| [TDMMethod](/TDMmethod.md) | Recommended |
| [relationType](/components_relationType.md) | Recommended |
| [relatedResource](/components_relatedResource.md) | Mandatory upon conditions |



