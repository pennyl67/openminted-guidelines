## Achieving compatibility with OpenMinTeD and interoperability across TDM resources

To be **fully compatible with OpenMinTeD**, you must endorse the following rules

* **Licensing**: 
  * You must ensure that the publications are_** distributed under Open Access conditions**_
  * You must include in the metadata record of each publication _**a link to the licence document**_ that describes the terms and conditions under which it is provided, and attach the licence document together with the publication; using a standard licence, such as [Creative Commons](https://creativecommons.org/share-your-work/) the most recent version, is recommended
* **Unique and persistent identifiers**:
  * If you already have a _**PID for your publication**_ \(preferably DOI\), make sure it is included in the metadata record \(cf. [identifier](/publications_identifier.md) for more information on identifier schemes\).

If you wish your material to be **easily processable and interoperable with TDM tools and services**, you should adopt the following **recommendations**:

* **Data formats**: The preferred formats for delivering textual material are **plain text, PDF** \(not proprietary and certainly not of scanned images\), and **XML**, which can be read by one of the readers offered in OpenMinTeD. If appropriate for your material, use one of the more specific data formats that are already supported by readers and converters included in the OpenMinTeD registry \(cf. [dataFormat](/dataFormat.md)\).

* **Character encoding**: The preferred character encoding is UTF-8.

* **Structural markup**: Further adoption of standards such as the [JATS article tag suite](https://jats.nlm.nih.gov/index.html) or [TEI P5 guidelines](http://www.tei-c.org/Guidelines/P5/) for annotating the internal structure of documents is recommended.

* **Domain classification**: Use standard classification vocabularies, such as [MeSH](https://www.nlm.nih.gov/mesh/), [DDC](https://www.oclc.org/dewey.en.html), [LCSH](http://id.loc.gov/authorities/subjects.html) etc., for adding classification tags to your material and specify the vocabulary you use in the metadata record; provide at least one broad category for your material \(e.g. life sciences, computing etc.\).

* **Linking through authority lists**: In all cases, where linking to other resources or entities \(e.g. persons, projects etc.\) in the metadata records is added, please try to do this through unique and persistent identifiers of authority lists and sources \(e.g. ORCID for persons, ISNI or fundref for organizations\), to the extent possible, documenting also the authority and/or scheme it adheres to.

* **Annotation formats**: If you want to** **provide **annotated publications**, please note that OpenMinTeD has endorsed the use of the [_**XML Metadata Interchange**_](http://www.omg.org/spec/XMI/)_** \(XMI\) format**_, specifically the representation of a [UIMA CAS](https://uima.apache.org/d/uimaj-2.9.0/references.html#ugr.ref.xmi) to encode annotations on text in particular when exchanging data between components within a workflow; the [_**Web Annotation**_](https://www.w3.org/annotation/) standard will be used to make annotations produced by OpenMinTeD workflows accessible to third parties and to encode annotations above the text level, e.g. on document/collection level.

Please, note that not all of the above requirements are absolute: if your material is not compliant with them, it may still be processable, but their adoption makes it better equipped for TDM and NLP processing.



