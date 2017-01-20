## Recommended schema for s/w resources {#recommended-schema-for-s-w-resources}

This section includes a synopsis of the recommended schema for s/w resources, i.e. the subset of M(andatory) and strongly R(ecommended) metadata elements, only as regards elements related to the resource itself. Additional elements required for the management of the metadata record (e.g. _metadataCreationDate, metadataCreator_ etc.) are not presented here, as they are to be handled by the OMTD platform.

| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](resourceType.md) | M | 
| [resourceName](resourceName.md) | M | 
| [description](description.md) | M | 
| [identifier](identifier.md) | M | 
| [version](version.md) | M | 
| [componentDistributionMedium](componentDistributionMedium.md) | M | 
| [componentType](componentType.md) | M | 
| [licence](licence.md) or [rightsStmtName](rightsStmtName.md) &amp; [rightsStmtURL](rightsStmtURL.md) \(one of the two must be provided\) | M | 
| [version of licence](version_of_licence.md) | M | 
| [contactEmail](contactEmail.md) or [landingPage](landingPage.md) \(one of the two must be provided\) | M | 
| [contactPerson](contactPerson.md) \(identifier or personName\) | R | 
| [contactGroup](contactGroup.md) \(identifier or organizationName\) | R | 
| [mailingList](mailingList.md) \(mailingListName, subscribe, unsubscribe, post, archive, otherArchive\) | R | 
| [issueTracker](issueTracker.md) | R | 
| [onlineHelpURL](onlineHelpURL.md) | R | 
| [mustBeCitedWith](mustBeCitedWith.md) | R | 
| [downloadURL](downloadURL.md) or [accessURL](accessURL.md) \(one of the two should be provided\) | M when applicable | 
| [resourceCreator](resourceCreator.md) \(person or organization, described with identifier or name\) | R | 
| [mediaType inside inputContentResourceInfo or outputResourceInfo \(i.e. mediaType of input and output resource\)](mediaType_inside_inputContentResourceInfo_or_outputResourceInfo.md) | M when applicable | 
| [resourceType inside inputContentResourceInfo or outputResourceInfo](resourceType_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable | 
| [language inside inputContentResourceInfo or outputResourceInfo](language_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable | 
| [characterEncoding inside inputContentResourceInfo or outputResourceInfo](characterEncoding_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable | 
| [mimeType inside inputContentResourceInfo or outputResourceInfo](mimeType_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable | 
| [dataFormatSpecific inside inputContentResourceInfo or outputResourceInfo](dataFormatSpecific_inside_inputContentResourceInfo_or_outputResourceInfo.md) | R when applicable | 
| [inputContentResourceInfo or outputContentResourceInfo/typesystem](inputContentResourceInfo or outputContentResourceInfo/typesystem.md) | R when applicable | 
| [inputContentResourceInfo or outputContentResourceInfo/tagset](inputContentResourceInfo or outputContentResourceInfo/tagset.md) | R when applicable | 
| [inputContentResourceInfo or outputContentResourceInfo/annotationLevel](inputContentResourceInfo or outputContentResourceInfo/annotationLevel.md) | R when applicable | 
| [typesystem](typesystem.md) | R | 
| [tagset](tagset.md) | R | 
| [annotationResource](annotationResource.md) | R | 
| [framework](framework.md) | R | 
| [for parameters: parameterName, description, parameterType, mandatory, multiValue](for parameters: parameterName, description, parameterType, mandatory, multiValue.md) | M when applicable | 
| [relationType=isCompatibleWith (external relation; link to models, annotation resources etc. that can be used with the component)](relationType=isCompatibleWith (external relation; link to models, annotation resources etc. that can be used with the component).md) | R | 
