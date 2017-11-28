#### resourceCreator
##### Usage
Recommended
##### Type
free text
##### Attributes
-
##### Definition/Explanations
Groups information on the person(s), group(s) or organization(s) that has/have created the resource
##### Recommended usage
You must first select "actorType" to indicate whether the resourceCreator is a person, group or organization. Depending on your choice, please fill in the appropriate details.
The recommended way for referring to a person is by giving their surname, given name and identifier (preferably the ORCID). 
For organizations, if possible, please also provide their identifier (e.g. ISNI).
The element can also be repeated to encode multiple persons/organizations.  
For corpora created through the OMTD corpus building process, the resource creator is considered to be the person that has put together the corpus through the user query.
##### Relation to other metadata schemas
* **DCMI:** skos:closeMatch dct:creator
* **DataCite 4.0:** skos:closeMatch datacite:Creator with datacite:creatorName (familyName & givenName) or datacite:nameIdentifier & datacite:nameIdentifierScheme & datacite:schemeURI
