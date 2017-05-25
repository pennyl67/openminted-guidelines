#### author

##### Usage

Recommended

##### Type

person

##### Attributes

ms:personIdentifierSchemeName \(for identifiers\) or xs:lang \(for name\)

##### Definition/Explanations

Groups information on the person\(s\) that has/have authored the publication

##### Recommended usage

The recommended way for referring to a person is by giving their surname and given name\(s\) as well as their identifier, preferably the ORCID; if you provide the identifier, please select also the relevant value from the list of values in the attribute "personIdentifierSchemeName"; if none is appropriate, please select "other" and use the "schemeURI" attribute to provide a link to a URL with more information about the identifier scheme.   
You may provide the name, preferably in the format "Surname, First name" at least in English; if you want to add names in other languages, you can use the “lang” attribute.   
The element can also be repeated to encode multiple persons.

##### Relation to other metadata schemas

* **OpenAIRE current version:** rels/rel
* **OpenAIRE v4.0:** datacite:creator
* **CORE:** article.authors
* **DCMI:** skos:closeMatch dct:creator
* **DataCite 4.0:** skos:closeMatch datacite:Creator with datacite:creatorName \(familyName & givenName\) or datacite:nameIdentifier & datacite:nameIdentifierScheme & datacite:schemeURI



