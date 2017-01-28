#### collectedFrom repositoryName or repositoryIdentifier
##### Usage
Recommended
##### Type
identifier (repositoryIdentifier) or multilingual free text (repositoryName)
##### Attributes
ms-omtd:repositoryIdentifierSchemeName (for identifiers) or xs:lang (for title)
##### Definition/Explanations
Refers to the entity (repository, aggregator etc.) from which the metadata record has been harvested into OMTD
##### Recommended usage
The recommended way for referring to a repository is by giving its identifier (e.g. openDOAR); if you provide the identifier, please select also the relevant value from the list of values in the attribute "repositoryIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 
If you don't know the identifier of the repository, you may provide the name at least in English; if you want to add names in other languages, you can use the “lang” attribute.
##### Relation to other metadata schemas
* **OpenAIRE v4.0:** dc:source
