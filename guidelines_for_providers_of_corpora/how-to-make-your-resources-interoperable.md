### How to comply with OpenMinTeD interoperability specifications

In order to ensure that your corpora can be mined in the OpenMinTeD platform, you must follow the same requirements that are set for scholarly publications. 

####Minimum requirements
At present, the [OpenMinTeD platform](https://services.openminted.eu) supports the following:
* **Data formats**: The preferred formats for delivering textual material are _**plain text, PDF **_\(not proprietary and certainly not of scanned images\), **XML**, which can be read by one of the readers offered in the OpenMinTeD platform; if appropriate for your material, use one of the more specific data formats that are already covered by readers and converters \(cf. [dataFormat](/dataFormat.md)\).
* **Character encoding**: The preferred character encoding is _**UTF-8**_.

####Recommendations
To be **fully compliant with OpenMinTeD**, you must implement the following conditions:
* **Licensing**:
  * You must ensure that the corpus is distributed under _**Open Access conditions**_
  * Please, include in the metadata record a _**link to the licence**_ document that describes the terms and conditions under which it is provided, and attach the licence document together with the resource.
  
{% blurb style='tip'%}
Please note that 
* using a standard licence, such as [Creative Commons](https://creativecommons.org/share-your-work/) the most recent version, is recommended for data resources
* you can use the [licence compatibility matrix](https://openminted.github.io/releases/license-matrix/) to check whether the licences of the single documents are compatible.
{% endblurb %}

* **Unique and persistent identifiers**:
  * If you already have a _**PID**_** **for your corpus \(preferably DOI\), make sure it is _**included in the metadata record**_ \(cf. [identifier](/corpora_identifier.md) for more information on identifier schemes\).

In addition, the following **recommendations contribute to interoperability and make your corpora easier to process**. If you fail to abide to them, it might still be possible to process your corpora via the OpenMinTeD platform, but this cannot be guaranteed and interoperability with other resources will suffer loss.

* **Structural markup**: Further adoption of standards such as the [JATS article tag suite](https://jats.nlm.nih.gov/index.html) or [TEI P5 guidelines](http://www.tei-c.org/Guidelines/P5/) for annotating the inner structure of texts is recommended.
* **Versioning**: Please, ensure that you version all your resources and label the versions in an unambiguous way, preferably following the [Semantic Versioning recommendations](https://semver.org/).
* **Documentation**: It is important that you provide the appropriate documentation for your resource \(e.g. publications about the design and construction of the corpus etc.\), which you should also version along with the corpus and add as reference to your metadata record.
* **Citation**: 
  * Make sure that you fill in the metadata record all the elements required for _**citing your resource**_[^1], i.e. the creator of the resource, a title, the resource type and an identifier, and optionally, the publication date, the version and the publisher or distributor.
  * You can also _**recommend one of the publications**_ about your resource as the one to be cited for scholarly attribution and add this information in the metadata record.
* **Domain classification**: Use _**standard classification vocabularies **_\(e.g. [MeSH](https://www.nlm.nih.gov/mesh/), [DDC](https://www.oclc.org/dewey.en.html), [LCSH](http://id.loc.gov/authorities/subjects.html) etc.\) for adding classification tags to your material and specify the vocabulary you use in the metadata record; provide at least one broad category for your material \(e.g. life sciences, computing etc.\).
* **Linking to other entities**: In all cases, where linking to other resources or entities \(e.g. persons, projects Letc.\) in the metadata records is added, please try to do this _**through unique and persistent identifiers of authority lists and sources**_, to the extent possible, documenting also the authority and/or scheme it adheres to.

{% blurb style='warning'%}
Please, note that there are no specifications yet for corpora to be used for ancillary purposes \(e.g. for training a tool\), as these are dependent on the requirements of the software that will use them and on the purpose of use.
{% endblurb %}

---

[^1] For citation, OpenMinTeD endorses the [Joint Declaration of Data Citation Principles](https://www.force11.org/group/joint-declaration-data-citation-principles-final), as well as the more specialised [RDA recommendations for data citation of evolving data](https://www.rd-alliance.org/system/files/RDA-DC-Recommendations_151020.pdf) and [DataCite guidelines](https://www.datacite.org/cite-your-data.html).

