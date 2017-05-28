## ​Recommended schema for ​lexical/conceptual resources, incl. annotation resources {#recommended-schema-for-lexical-conceptual-resources}
The following sections include a synopsis of the minimal schemas  for ancillary knowledge resources, i.e. the subset of M(andatory) and strongly R(ecommended) metadata elements per resource type, given that knowledge resources may take one of the following resource types:

*   **lexical/conceptual resource**: reserved not only for lexica, ontologies, term lists, glossaries etc. but also for any resource that can be used for annotation purposes, i.e. linguistic tagsets, typesystems etc.
*   **language description**: reserved mainly for computational grammars and for ML models.

It should also be noted that additional elements required for the management of the metadata record (e.g. _metadataCreationDate, metadataCreator_ etc.) are not presented here, as they are to be handled by the OMTD platform.


| OMTD-SHARE element | Usage |
| --- | --- |
| [resourceType](\lcr_resourceType.md) | M |
| [resourceName](\lcr_resourceName.md) | M |
| [description](\lcr_description.md) | M |
| [identifier](\lcr_identifier.md) | M |
| [version](\lcr_version.md) | M |
| [distributionMedium](\lcr_distributionMedium.md) | M |
| [licence](\lcr_licence.md) or [rightsStmtName](\lcr_rightsStmtName.md) & [rightsStmtURL](\lcr_rightsStmtUrl.md) \(one of the two must be provided\)\] | M |
| [version of licence](\lcr_version_of_licence.md) | M |
| [distributionMedium](\lcr_distributionMedium.md) | M |
| [downloadURL](\lcr_downloadURL.md) | M when applicable |
| [contactEmail](\lcr_contactEmail.md) or [landingPage](\lcr_landingPage.md) \(one of the two must be provided\) | M |
| [contactPerson](\lcr_contactPerson.md) \(identifier or personName\) | R |
| [contactGroup](\lcr_contactGroup.md) \(identifier or organizationName\) | R |
| [mustBeCitedWith](\lcr_mustBeCitedWith.md) | R |
| [lexicalConceptualResourceType](\lcr_lexicalConceptualResourceType.md) | M |
| [encodingLevel](\lcr_encodingLevel.md) | R |
| [linguisticInformation](\lcr_linguisticInformation.md) | R |
| [conformanceToStandardsBestPractices](\lcr_conformanceToStandardsBestPractices.md) | R |
| [lingualityType](\lcr_lingualityType.md) | M |
| [language](\lcr_language.md) | M |
| [metalanguage](\lcr_metalanguage.md) | R |
| [size](\lcr_size.md) & sizeUnit | M |
| [mimeType](\lcr_mimeType.md) | R |
| [characterEncoding](\lcr_characterEncoding.md) | R |
| [domain](\lcr_domain.md) | R |
| [relationType](\lcr_relationType.md) | R |
| [relatedResource1](\lcr_relatedResource1.md) | R |
| [relatedResource2](\lcr_relatedResource2.md) | R |



