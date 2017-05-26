### Achieving compatibility with OpenMinTeD and interoperability across TDM resources {#how-to-make-your-resources-interoperable}

In order to ensure that your corpora can be mined in the OpenMinTeD platform, you must follow the same requirements that are set for scholarly publications. You must therefore

* provide direct access to the contents of each corpus
* describe each corpus with a metadata record compatible with the [OTMD-SHARE minimal schema](/guidelines_for_providers_of_corpora/recommended_schema_for_corpora.md).

To be **fully compliant with OpenMinTeD**, you must

* ensure that the corpus is distributed under Open Access conditions
* include in the metadata record a link to the licence document that describes the terms and conditions under which it is provided, and attach the licence document together with the resource; using a standard licence, such as Creative Commons the most recent version, is recommended
* if you already have a PID for your publication \(preferably DOI\), make sure it is included in the metadata record \(cf. [identifier](/corpora_identifier.md) for more information on identifier schemes\).


In addition, the following **recommendations contribute to interoperability and make your corpora easier to process**. If you fail to abide to them, it might still be possible to process your corpora via the OpenMinTeD platform, but this cannot be guaranteed and interoperability with other resources will suffer loss.

So, if you intend to create a new corpus, it is important that you take into account from the early steps of its design, the requirements, standards, best practices and recommendations promoted by OpenMinTeD and other cooperating infrastructures.


* The preferred **formats **for delivering textual material are plain text, XML, PDF \(not proprietary and certainly not of scanned images\), which can be read by one of the existing readers.

* If appropriate for your material, use one of the more specific **data formats **that are already covered by readers and converters \(cf. [dataFormat](/corpora_dataFormat)\).

* The preferred **character encoding** is UTF-8.

* Further adoption of standards such as the [JATS article tag suite](https://jats.nlm.nih.gov/index.html) or [TEI P5 guidelines](http://www.tei-c.org/Guidelines/P5/) for annotating the inner structure of texts is recommended.
* Please, ensure that you version all your resources and label the versions in an unambiguous way, preferably following the [Semantic Versioning recommendations](http://semver.org/).
* It is important that you provide the appropriate documentation for your resource \(e.g. publications about the design and construction of the corpus etc.\), which you should also version along with the corpus and add as reference to your metadata record.
* Recommend one of the publications about your resource as the one to be cited for scholarly attribution and add this information in the metadata record.
* Make sure that you fill in the metadata record all the elements required for citing your resource[^1], i.e. the creator of the resource, a title, the resource type and an identifier, and optionally, the publication date, the version and the publisher or distributor.
* Use standard classification vocabularies \(e.g. [MeSH](https://www.nlm.nih.gov/mesh/), [DDC](https://www.oclc.org/dewey.en.html), [LCSH](http://id.loc.gov/authorities/subjects.html) etc.\) for adding classification tags to your material and specify the vocabulary you use in the metadata record; provide at least one broad category for your material \(e.g. life sciences, computing etc.\).
* In all cases, where linking to other resources or entities \(e.g. persons, projects etc.\) in the metadata records is added, please try to do this through unique and persistent identifiers of authority lists and sources, to the extent possible, documenting also the authority and/or scheme it adheres to.

Please, note that there are no general requirements yet for corpora to be used for ancillary purposes \(e.g. for training a tool\), as these are dependent on the requirements of the software that will use them and on the purpose of use.


---

[^1] For citation, OpenMinTeD endorses the [Joint Declaration of Data Citation Principles](https://www.force11.org/group/joint-declaration-data-citation-principles-final), as well as the more specialised [RDA recommendations for data citation of evolving data](https://www.rd-alliance.org/system/files/RDA-DC-Recommendations_151020.pdf) and [DataCite guidelines](https://www.datacite.org/cite-your-data.html).

