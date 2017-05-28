#### version

##### Usage
Mandatory upon conditions

##### Usage conditions
either version or versionDate must be filled in

##### Type
numerical pattern

##### Definition/Explanations
Associates a resource with a numeric pattern of the form major_version.minor_version.patch (in accordance to the semantic versioning guidelines, cf. http://semver.org\) that identifies its version

##### Recommended usage
Please, keep this only for versions of the same resource (e.g. corrected, enlarged etc.) and not for variants or for versions with additional or different information (e.g. annotated versions). 
The recommended practice for versioning should follow semantic versioning guidelines (http://semver.org/)
The alternative element versionDate should be used only for resources whose version is unknown.

##### Relation to other metadata schemas
* **DCMI:** skos:exactMatch dct:hasVersion
* **DataCite 4.0:** skos:exactMatch datacite:Version
