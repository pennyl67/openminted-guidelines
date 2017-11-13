### Sharing web services through OpenMinTeD

**Step 1**

If you intend to share your TDM software as a web service through OpenMinTeD, please ensure that you comply with the specifications at [https://openminted.github.io/releases/processing-web-services/1.0.0/specification](https://openminted.github.io/releases/processing-web-services/1.0.0/specification). 



Step 2: You can then visit the OpenMinTeD registry where you can register your web service in one of the following ways:

* edit from scratch the OMTD-SHARE metadata record using the OpenMinTeD editor or
* upload an XML file with the OMTD-SHARE metadata record 

You must provide the the URL where the web service can be executed in the metadata element _&lt;distributionLocation&gt;_, e.g.

`<distributionLocation>http://nactem.ac.uk/api/openminted/chebi</distributionLocation>`

In all of these cases, the metadata record can be viewed and edited at the end of the process.

