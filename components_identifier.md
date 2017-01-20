#### identifier
##### Usage
Mandatory
##### Type
free text
##### Attributes
ms:resourceIdentifierSchemeName or ms:schemeURI
##### Definition/Explanations
Reference to a PID, DOI or any kind of identifier used by the resource provider for the resource
##### Recommended usage
Provide a unique identifier already assigned by an authoritative source; you can use either
##### Relation to other metadata schema elements
* **Maven POM 4.0.0:** groupId & artifcactId & version & packaging & classifier, with resourceIdentifierSchemeURI="https://maven.apache.org/pom.html#Maven_Coordinates"
* **GATE:** class 
* **UIMA/UIMA-fit:** class
* **DCMI:** skos:narrowMatch dct:identifier
* **DataCite 4.0:** skos:broadMatch datacite:identifier (identifierType can only be DOI)
