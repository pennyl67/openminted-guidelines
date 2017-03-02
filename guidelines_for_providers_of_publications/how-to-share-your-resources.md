### How to register your resources {#how-to-share-your-resources}

Interested content providers must implement a Java interface, called **ContentConnector**, which can be found at [https://github.com/openminted/content-connector-api](https://github.com/openminted/content-connector-api). The implementation is then included in the code of the ContentService of the OpenMinTeD platform. This interface specifies three methods:

* _**search**_, which accepts a Query object describing a query and returns a page of metadata. This method is used for browsing the metadata of the provider and supports keyword search, advanced search in a number of fields and also faceted search. The result of the method is \(a\) a page \(of user specified size\) of metadata, \(b\) the statistics of the results \(total number of hits, etc\), and \(c\) the facets \(if requested\).

* _**fetchMetadata**_, which accepts a Query, but, unlike the previous method, returns all the metadata of the result, without any statistics or facets. The result is a stream containing a single xml element \(called “publications”\), which in turn contains all the metadata of the content. This method is called when a corpus is being built.

* _**downloadFullText**_, which given a publication identifier \(as contained in the metadata\) returns a stream containing the actual content. This method is again used when the platform is building a corpus.

Additional technical information is provided in the Java code of the interface.

