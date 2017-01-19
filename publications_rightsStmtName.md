#### rightsStmtName
##### Usage
Mandatory under conditions
##### Conditions for usage
either licence or rightsStmt must be filled in
##### Type
open controlled vocabulary
##### Controlled vocabulary reference and/or values
ms-omtd:rightsStmtName: _openAccess_, _closedAccess_, _embargoedAccess_, _restrictedAccess_
##### Definition/Explanations
The name of an official statement indicative of licensing terms for the use of a resource (e.g. open access, free to read etc.); its semantics should be clear, preferrably formally expressed and stored at a url.

The current list of predefined values comes from OpenAIRE, but it's under revision.
##### Recommended usage
The "rightsStmtName" and "rightsStmtURL" elements can be used in addition to the "licence" value in order to facilitate users to understand the licensing terms of a resource.
##### Relation to other metadata schema elements
* **OpenAIRE current version:** conversion from bestlicence classname
* **DCMI:** skos:closeMatch dct:accessRights
* **DataCite 4.0:** skos:closeMatch datacite:rights
