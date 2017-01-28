#### originalDataProviderJournal
##### Usage
Recommended under conditions
##### Conditions for usage
if originalDataProviderType=journal
##### Type
identifier or multilingual free text
##### Attributes
ms-omtd:journalIdentifierSchemeName (for identifiers) or xs:lang (for title)
##### Definition/Explanations
Refers to the journal from which the metadata record has been harvested
##### Recommended usage
The recommended way for referring to a journal is by giving their identifier (e.g. ISSN, DOI); if you provide the identifier, please select also the relevant value from the list of values in the attribute "journalIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme. 
If you don't know the identifier of the journal, you may provide the title at least in English; if you want to add titles in other languages, you can use the “lang” attribute.
##### Relation to other metadata schemas
* **OpenAIRE current version:** collectedFrom
* **CORE:** article.journals
* **DCMI:** skos:narrowMatch dct:source
