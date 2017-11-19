#### resourceIdentifier

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
  ##### Relation to other metadata schemas
* **DCMI:** skos:closeMatch dct:identifier
* **DataCite 4.0:** skos:broadMatch datacite:identifier \(identifierType can only be DOI\)



