### Recommended schema for software resources {#recommended-schema-for-s-w-resources}

This section includes a synopsis of the recommended schema for sofware resources, i.e. the subset of Mandatory and strongly Recommended metadata elements, only as regards elements related to the resource itself. Additional elements required for the management of the metadata record \(e.g. _metadataCreationDate, metadataCreator_ etc.\) are not presented here, as they are to be handled by the OMTD platform.

| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](/components_resourceType.md) | Mandatory |
| [resourceName](/components_resourceName.md) | Mandatory |
| [description](/components_description.md) | Mandatory |
| [identifier](/components_identifier.md) | Mandatory |
| [public](/public)\` | Mandatory |
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
| [downloadURL](/components_downloadURL.md) or [accessURL](/components_accessURL.md) | Mandatory \(choice: one element should be encoded\) |
| [command](/components_command.md) | Mandatory upon conditions |
| [licence](/components_licence.md) or [rightsStatement](/components_rightsStatement.md) | Mandatory \(choice: one element must be encoded\) |
| [nonStandardLicenceName](/components_nonStandardLicenceName.md) and  [nonStandardLicenceTermsURL](/components_nonStandardLicenceTermsURL.md) | Mandatory upon conditions |
| [processingResourceType](/components_resourceType_inside_inputContentResourceInfo_or_outputResourceInfo.md) inside inputContentResourceInfo or outputResourceInfo | Mandatory when applicable |
| [dataFormat](/components_dataFormatSpecific_inside_inputContentResourceInfo_or_outputResourceInfo.md) inside inputContentResourceInfo or outputResourceInfo | Recommended when applicable |
| [language](/components_language_inside_inputContentResourceInfo_or_outputResourceInfo.md) inside inputContentResourceInfo or outputResourceInfo | Recommended when applicable |
| [annotationLevel](/components_annotationLevel_inside_inputContentResourceInfo_or_outputResourceInfo.md) inside inputContentResourceInfo or outputResourceInfo | Recommended when applicable |
| for parameters: [parameterName](/components_parameterName), [parameterLabel](/components_parameterLabel), [parameterDescription](/components_parameterDescription), [parameterType](/components_parameterType), [optional](/components_optional), [multiValue](/components_multiValue), [defaultValue](/components_defaultValue) | Mandatory when applicable |
| [typesystem](/components_typesystem_inside_componentDependencies.md) inside componentDependencies | Recommended |
| [annotationSchema](/components_anotationSchema_inside_componentDependencies.md) inside componentDependencies | Recommended |
| [annotationResource](/components_annotationResource_inside_componentDependencies.md) inside componentDependencies | Recommended |
| [framework](/components_framework.md) | Mandatory |
| [relationType](/compoments_relationType.md) | Recommended |
| [relatedResource](/compoments_relatedResource.md) | Mandatory upon conditions |



