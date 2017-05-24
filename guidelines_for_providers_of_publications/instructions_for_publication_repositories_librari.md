## Instructions for publication repositories, libraries, journals, publishers, etc. {#instructions-for-publication-repositories-libraries-journals-publishers-etc}

### How to register your resources {#uploading-instructions}

If you wish to register publications that can be harvested for TDM purposes through OpenMinTeD, you can do so

* by registering through [OpenAIRE](http://www.openaire.eu), following procedures and guidelines at: [https://www.openaire.eu/validator/welcome.action](https://www.openaire.eu/validator/welcome.action)

OR

* by registering through [CORE](http://core.ac.uk), following procedures at: [https://core.ac.uk/join](https://core.ac.uk/join)
~~
Add here procedure for content connector:
the content connector that has been built in the OpenMinTeD framework that allows harvesting of open access publications through the APIs of publishers that allow this. further info or requirements for this?~~


### Minimal requirements

For each publication, you must deliver:
* a file with the **full text** 
* a **metadata description** with at least bibliographic information about it, in preference following the ~~OpenAIRE guidelines~~; these metadata elements are used for building a faceted view of the federated content (see ~~link~~ for more information on the deployment of publications in OpenMinTeD) .

(compatible with the ~~OMTD-SHARE minimal schema~~) 
To be fully compatible with OpenMinTeD, you must
* ensure that the publications are distributed under Open Access conditions
* include in the metadata record of each publication a link to the licence document that describes the terms and conditions under which it is provided, and attach the licence document together with the publication
* if you already have a PID for your publication \(preferably DOI\), make sure it is included in the metadata record \(cf. [identifier](/publications_identifier.md) for more information on identifier schemes\).


### Further recommendations
If you wish your material to be easily processable and interoperable with TDM tools and services, you should adopt the following recommendations:

* The preferred **formats** for delivering textual material are plain text, XML, PDF \(not proprietary and certainly not of scanned images\), which can be read by one of the existing readers.

* If appropriate for your material, use one of the **more specific data formats** that are already supported by readers and converters included in the OpenMinTeD registry \(cf. [dataFormatSpecific](/components_dataFormatSpecific_inside_inputContentResourceInfo_or_outputResourceInfo.md%29\)\).

* The preferred **character encoding** is UTF-8.


* Further adoption of standards such as the [JATS article tag suite](https://jats.nlm.nih.gov/index.html) or [TEI P5 guidelines](http://www.tei-c.org/Guidelines/P5/) for annotating the inner structure of publications is recommended.
* Use standard classification vocabularies, such as [MeSH](https://www.nlm.nih.gov/mesh/), [DDC](https://www.oclc.org/dewey.en.html), [LCSH](http://id.loc.gov/authorities/subjects.html) etc.\) for adding classification tags to your material and specify the vocabulary you use in the metadata record; provide at least one broad category for your material \(e.g. life sciences, computing etc.\).
* In all cases, where linking to other resources or entities \(e.g. persons, projects etc.\) in the metadata records is added, please try to do this through unique and persistent identifiers of authority lists and sources, to the extent possible, documenting also the authority and/or scheme it adheres to.





Please, note that not all of the above requirements are absolute: if your material is not compliant with them, it may still be processable, but their adoption makes it better equipped for TDM and NLP processing.


