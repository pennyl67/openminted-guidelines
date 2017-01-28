#### originalDataProviderRepository
##### Usage
Recommended under conditions
##### Conditions for usage
if originalDataProviderType=repository
##### Type
identifier or multilingual free text
##### Attributes
ms-omtd:repositoryIdentifierSchemeName (for identifiers) or xs:lang (for title)
##### Definition/Explanations
Refers to the entity (repository, aggregator etc.) from which the metadata record has been harvested
##### Recommended usage
The recommended way for referring to a repository is by giving their identifier (e.g. from OpenDOAR, re3data etc.); if you provide the identifier, please select also the relevant value from the list of values in the attribute "repositoryIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 
If you don't know the identifier of the repository, you may provide the name at least in English; if you want to add names in other languages, you can use the “lang” attribute.
##### Relation to other metadata schemas
* **OpenAIRE current version:** collectedFrom
* **CORE:** article.repositories
* **DCMI:** skos:narrowMatch dct:source
