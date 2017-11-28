#### relationType

##### Usage

Recommended

##### Type

Open controlled vocabulary

##### Controlled vocabulary reference and/or values

ms:relationType: _isPartOf_, _isPartWith_, _hasPart_, _hasOutcome_, _isCombinedWith_, _requiresLR_, _requiresSoftware_, _isexactMatch_, _isSimilarTo_, _isContinuationOf_, _isVersionOf_, _replaces_, _isReplacedWith_, _isCreatedBy_, _isElicitedBy_, _isRecordedBy_, _isEditedBy_, _isAnalysedBy_, _isEvaluatedBy_, _isQueriedBy_, _isAccessedBy_, _isArchivedBy_, _isDisplayedBy_, _isCompatibleWith, isAnnotatedVersionOf, hasAnnotatedVersion_

##### Definition/Explanations

Specifies the type of relation holding between two entities \(e.g. two resources that comprise one new resource together, a corpus and the s/w component that has been used for its creation or a corpus and the publication that describes it\)

##### Recommended usage
Annotated corpora must be linked to the raw corpus (as relatedResource) through the relationType with value isAnnotatedVersion.

##### Relation to other metadata schemasc
* **DataCite 4.0:** skos:closeMatch datacite:relationType



