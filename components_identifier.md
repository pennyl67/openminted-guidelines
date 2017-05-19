#### identifier

##### Usage

Mandatory

##### Type

free text

##### Attributes

ms:resourceIdentifierSchemeName or ms:schemeURI

##### Definition/Explanations

Associates a resource to an identifier \(e.g. PID, DOI, internal to an organization etc.\), i.e. a string used to uniquely identify it.

##### Recommended usage

For **components stored in Maven**, the Maven id must be used with a reference to the Maven scheme \(resourceIdentifierSchemeName="maven"\). This is combined with the Java fully qualified class naming conventions to give the following coordinates: groupId:artifactId:version:\(packaging\):\(classifier\)\#class.

For other components, if they already have a unique identifier assigned by an authoritative source \(e.g. DOI\), please provide this together with the following:

* use the attribute "resourceIdentifierSchemeName" to specify the scheme, by selecting one of the pre-defined values \(e.g. DOI, HDL, ISLRN etc.\) or,
* if the scheme is not listed among them, select the "other" value and use the attribute "schemeURI" to provide a link to the URL that documents the scheme it adheres to. 

If the resource doesn't have a unique identifier, an identifier will be assigned by OpenMinTeD. 

**Relation to other metadata schemas**

* **Maven POM 4.0.0:** groupId & artifcactId & version & packaging & classifier, with resourceIdentifierSchemeName="maven"
* **GATE:** class 
* **UIMA/UIMA-fit:** class
* **DCMI:** skos:narrowMatch dct:identifier
* **DataCite 4.0:** skos:broadMatch datacite:identifier \(identifierType can only be DOI\)



