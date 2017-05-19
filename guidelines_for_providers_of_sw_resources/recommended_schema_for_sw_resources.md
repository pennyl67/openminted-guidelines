## Recommended schema for software resources {#recommended-schema-for-s-w-resources}

This section includes a synopsis of the recommended schema for sofware resources, i.e. the subset of M\(andatory\) and strongly R\(ecommended\) metadata elements, only as regards elements related to the resource itself. Additional elements required for the management of the metadata record \(e.g. _metadataCreationDate, metadataCreator_ etc.\) are not presented here, as they are to be handled by the OMTD platform.

| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](/components_resourceType.md) | Mandatory |
| [resourceName](/components_resourceName.md) | Mandatory |
| [description](/components_description.md) | Mandatory |
| [identifier](/components_identifier.md) | Mandatory |
| [public](/public)\` | Mandatory |
| [version](/components_version.md) or [versionDate](/versiondate.md) | Mandatory \(choice: one element must be encoded\) |
| [contactEmail](/components_contactEmail.md) or [landingPage ](/components_landingPage.md)or [contactPerson](/components_contactPerson.md) | Mandatory \(choice: one element must be encoded\) |
| [contactGroup](/components_contactGroup.md) | Recommended |
|  |  |
| [componentDistributionMedium](/components_componentDistributionMedium.md) | M |
| [componentType](/components_componentType.md) | M |
| [licence](/components_licence.md) or [rightsStmtName](/components_rightsStmtName.md) & [rightsStmtURL](/components_rightsStmtURL.md) \(one of the two must be provided\) | M |
| [version of licence](/components_version_of_licence.md) | M |
| [contactEmail](/components_contactEmail.md) or [landingPage](/components_landingPage.md) \(one of the two must be provided\) | M |
| [contactPerson](/components_contactPerson.md) \(identifier or personName\) | R |
| [contactGroup](/components_contactGroup.md) \(identifier or organizationName\) | R |
| [mailingList](/components_mailingList.md) \(mailingListName, subscribe, unsubscribe, post, archive, otherArchive\) | R |
| [issueTracker](/components_issueTracker.md) | R |
| [onlineHelpURL](/components_onlineHelpURL.md) | R |
| [mustBeCitedWith](/components_mustBeCitedWith.md) | R |
| [downloadURL](/components_downloadURL.md) or [accessURL](/components_accessURL.md) \(one of the two should be provided\) | M when applicable |
| [resourceCreator](/components_resourceCreator.md) \(person or organization, described with identifier or name\) | R |
| [mediaType inside inputContentResourceInfo or outputResourceInfo \(i.e. mediaType of input and output resource\)](/components_mediaType_inside_inputContentResourceInfo_or_outputResourceInfo.md) | M when applicable |
| [resourceType inside inputContentResourceInfo or outputResourceInfo](/components_resourceType_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable |
| [language inside inputContentResourceInfo or outputResourceInfo](/components_language_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable |
| [characterEncoding inside inputContentResourceInfo or outputResourceInfo](/components_characterEncoding_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable |
| [mimeType inside inputContentResourceInfo or outputResourceInfo](/components_mimeType_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable |
| [dataFormatSpecific inside inputContentResourceInfo or outputResourceInfo](/components_dataFormatSpecific_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable |
| [typesystem inside inputContentResourceInfo or outputResourceInfo](/components_typesystem_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable |
| [tagset inside inputContentResourceInfo or outputResourceInfo](/components_tagset_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable |
| [annotationLevel inside inputContentResourceInfo or outputResourceInfo](/components_annotationLevel_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable |
| [typesystem](/components_typesystem_inside_componentDependencies.md) | R |
| [tagset](/components_tagset_inside_componentDependencies.md) | R |
| [annotationResource](/components_annotationResource_inside_componentDependencies.md) | R |
| [framework](/components_framework.md) | R |
| for parameters: parameterName, description, parameterType, mandatory, multiValue | M when applicable |
| [relationType](/compoments_relationType.md) =isCompatibleWith \(external relation; link to models, annotation resources etc. that can be used with the component\) | R |



