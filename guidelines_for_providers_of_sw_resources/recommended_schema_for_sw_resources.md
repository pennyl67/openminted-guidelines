### Recommended schema for software resources {#recommended-schema-for-s-w-resources}

This section includes a synopsis of the recommended schema for sofware resources, i.e. the subset of Mandatory and strongly Recommended metadata elements, only as regards elements related to the resource itself. Additional elements required for the management of the metadata record \(e.g. _metadataCreationDate, metadataCreator_ etc.\) are not presented here, as they are to be handled by the OMTD platform.

The following table presents mandatory and recommended elements for Machine Learning models; these have been selected so as to help

* identify the resource and provide information about it \(e.g. resourceIdentifier, resourceName, version\)
* describe the legal terms for using the resource \(e.g. licence or rightsStatement\) 
* encode  technical features that are useful for achieving interoperability with content and ancillary knowledge resources \(e.g. componentType, application, input and output specifications and dependencies\)
* give access to the component and execute it \(e.g. distributionLocation, command\)
* classify the resource along a variety of criteria that end-users can apply for locating resources of interest for their research 
  \(e.g. componentType, applicationFunction, TDMMethod\)
* contribute to attribution, citation and reproducibility of experiments \(e.g. resourceCreator, mustBeCitedWith\).

| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](/components_resourceType.md) | Mandatory |
| [resourceName](/components_resourceName.md) | Mandatory |
| [description](/components_description.md) | Mandatory |
| [identifier](/components_identifier.md) | Mandatory |
| [public](/components_public.md) | Mandatory |
| [version](/components_version.md) | Mandatory |
| [contactEmail](/components_contactEmail.md) or [landingPage ](/components_landingPage.md)or [contactPerson](/components_contactPerson.md) | Mandatory \(choice: one element must be encoded\) |
| [contactGroup](/components_contactGroup.md) | Recommended |
| [mustBeCitedWith](/components_mustBeCitedWith.md) | Recommended |
| [onlineHelpURL](/components_onlineHelpURL.md) | Recommended |
| [resourceCreator](/components_resourceCreator.md) \(person or organization, described with identifier or name\) | Recommended |
| [componentType](/components_componentType.md) | Mandatory |
| [application](/components_application.md) | Mandatory |
| [applicationFunction](/components_applicationFunction.md) | Mandatory upon conditions |
| [componentDistributionForm](/components_componentDistributionForm.md) | Mandatory |
| [distributionLocation](/components_downloadURL) | Mandatory |
| [command](/components_command.md) | Mandatory upon conditions |
| [licence](/components_licence.md) or [rightsStatement](/components_rightsStatement.md) | Mandatory \(choice: one element must be encoded\) |
| [nonStandardLicenceName](/components_nonStandardLicenceName.md) and  [nonStandardLicenceTermsURL](/components_nonStandardLicenceTermsURL.md) | Mandatory upon conditions |
| [processingResourceType](/components_resourceType_inside_inputContentResourceInfo_or_outputResourceInfo.md) inside inputContentResourceInfo or outputResourceInfo | Mandatory when applicable |
| [dataFormat](/components_dataFormatSpecific_inside_inputContentResourceInfo_or_outputResourceInfo.md) inside inputContentResourceInfo or outputResourceInfo | Recommended when applicable |
| [language](/components_language_inside_inputContentResourceInfo_or_outputResourceInfo.md) inside inputContentResourceInfo or outputResourceInfo | Mandatory when applicable |
| [annotationLevel](/components_annotationLevel_inside_inputContentResourceInfo_or_outputResourceInfo.md) inside inputContentResourceInfo or outputResourceInfo | Mandatory when applicable |
| for parameters: [parameterName](/components_parameterName), [parameterLabel](/components_parameterLabel), [parameterDescription](/components_parameterDescription), [parameterType](/components_parameterType), [optional](/components_optional), [multiValue](/components_multiValue), [defaultValue](/components_defaultValue) | Mandatory when applicable |
| [typesystem](/components_typesystem_inside_componentDependencies.md) inside componentDependencies | Mandatory when applicable |
| [annotationSchema](/components_anotationSchema_inside_componentDependencies.md) inside componentDependencies | Recommended when applicable |
| [annotationResource](/components_annotationResource_inside_componentDependencies.md) inside componentDependencies | Recommended when applicable |
| [framework](/components_framework.md) | Mandatory |
| [relationType](/components_relationType.md) | Recommended |
| [relatedResource](/components_relatedResource.md) | Mandatory upon conditions |



