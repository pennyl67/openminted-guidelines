#### resourceIdentifier

##### Usage

Mandatory

##### Type

free text

##### Attributes

ms:resourceIdentifierSchemeName or ms:schemeURI

##### Definition/Explanations

Associates a resource to an identifier \(e.g. PID, DOI, id internal to an organization etc.\), i.e. a string used to uniquely identify it.

##### Recommended usage

* For **components shared through Maven**, the Maven id must be used; this is combined with the Java fully qualified class naming conventions to give the following coordinates: groupId:artifactId:version:\(packaging\):\(classifier\)\#class; e.g.

`<resourceIdentifier resourceIdentifierSchemeName="maven">mvn:de.tudarmstadt.ukp.dkpro.core:de.tudarmstadt.ukp.dkpro.core.berkeleyparser-gpl:1.9.0-SNAPSHOT#de.tudarmstadt.ukp.dkpro.core.berkeleyparser.BerkeleyParser</resourceIdentifier>`

* For **components shared as Docker images**, this should be the name used to invoke the component, e.g.

`<resourceIdentifier resourceIdentifierSchemeName="OMTD-docker">default.modules.simpleprojector</resourceIdentifier>`

* If a software resource already has a a unique identifier assigned by an authoritative source \(e.g. DOI\), please provide this together with the following: 
  * use the attribute "resourceIdentifierSchemeName" to specify the scheme, by selecting one of the pre-defined values \(e.g. DOI, HDL, ISLRN etc.\) or,
  * if the scheme is not listed among them, select the "other" value and use the attribute "schemeURI" to provide a link to the URL that documents the scheme it adheres to. 

If the resource doesn't have a unique identifier, an identifier will be assigned by OpenMinTeD.

**Relation to other metadata schemas**

* **Maven POM 4.0.0:** groupId & artifcactId & version & packaging & classifier, with resourceIdentifierSchemeName="maven"
* **GATE:** class 
* **UIMA/UIMA-fit:** class
* **DCMI:** skos:narrowMatch dct:identifier
* **DataCite 4.0:** skos:broadMatch datacite:identifier \(identifierType can only be DOI\)



