### ​How to make your knowledge resources interoperable {#how-to-make-your-knowledge-resources-interoperable}

In addition, if you want to be fully compliant with the OpenMinTeD interoperability requirements, please ensure that

* you provide the resource in a standard format, preferably XML or JSON-based syntax, or any other RDF serialisation format \(e.g. Turtle or N3\)
* all elements in the knowledge resource are identified with a URI; for Linked Data resources, the following identifiers should be used:
  * JSON-LD - the @id keyword
  * RDF/XML - the attributes xml:base, rdf:ID and rdf:about
  * XML - the xml:id attribute
* you register knowledge resources independently of any component that uses them, e.g. in a separate Maven artifact.

In the case that you provide the resource

* in another format, given that adherence to Linked Data standards is not imposed
* packaged in Maven artifacts with the components that use it, at the expense, however, of reusability

you still qualify for partial compliance.

