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
* the attribute "resourceIdentifierSchemeName" to specify the scheme, by selecting one of the pre-defined values \(e.g. DOI, HDL, ISLRN etc.\) or,
* if the scheme is not listed among them, select the "other" value and use the attribute "schemeURI" to provide a link to the URL that documents the scheme it adheres to. 
If the resource doesn't have a unique identifier, an identifier will be assigned by OpenMinTeD. 
For components harvested from Maven, the Maven id can be used with a reference to the Maven scheme \(https://maven.apache.org/pom.html#Maven_Coordinates\). This is combined with the Java fully qualified class naming conventions to give the following coordinates: groupId:artifactId:version:\(packaging\):\(classifier\)#class
##### Relation to other metadata schemas
* **Maven POM 4.0.0:** groupId & artifcactId & version & packaging & classifier, with resourceIdentifierSchemeURI="https://maven.apache.org/pom.html#Maven_Coordinates"
* **GATE:** class 
* **UIMA/UIMA-fit:** class
* **DCMI:** skos:narrowMatch dct:identifier
* **DataCite 4.0:** skos:broadMatch datacite:identifier (identifierType can only be DOI)
