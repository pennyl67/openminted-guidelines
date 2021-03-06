### How to share apps/components as web services

{% blurb style='warning'%}
**Don't forget!** Check that your software complies with **at least the minimal level** of the [OpenMinTeD interoperability requirements and recommendations](/guidelines_for_providers_of_sw_resources/how-to-make-your-components-interoperable.md).

In addition for web services, please keep in mind that we currently support only REST services.
{% endblurb %}



#### **Step 1 - Preparing and packaging**

If you intend to share your TDM software \(application or component\) as a web service through OpenMinTeD, please 
* ensure that it uses UIMA CAS XMI messaging system as specified at [https://openminted.github.io/releases/processing-web-services/1.0.0/specification](https://openminted.github.io/releases/processing-web-services/1.0.0/specification) and
* upload the typesystem that the web service deploys in Maven[^1].


#### **Step 2 - Adding in the OpenMinTeD platform**

You can then visit the [OpenMinTeD registry](https://services.openminted.eu/resourceRegistration/component) where you can register your web service in one of the following ways:

* edit from scratch the [OMTD-SHARE](/the_omtd-share_metadata_schema.md) metadata record[^2] using the OpenMinTeD editor or
* upload an XML file with the [OMTD-SHARE](/the_omtd-share_metadata_schema.md) metadata record. 

In both cases, as long as the metadata record is private (i.e. the metadata element "public" has the value "no"), it can be viewed and edited at the end of the process.


Please, note that in the metadata record, you must include
(1) the URL where the web service can be executed in the element **_distributionLocation_**, e.g.

`<distributionLocation>http://nactem.ac.uk/api/openminted/chebi</distributionLocation>`

(2) the typesystem details in the the module **_componentDependencies/typesystem_** and more specifically in the elements **_resourceName_** and **_resourceIdentifier_** (Maven coordinates), e.g.


`<resourceName>Chebi Curation Type System</resourceName>`

and

`<resourceIdentifier resourceIdentifierSchemeName="maven">mvn:uk.ac.nactem.uima:ChebiCurationTypeSystem:0.1</resourceIdentifier>`




--- 
[^1]: Please, note that for semantic interoperability reasons, OpenMinTeD recommends the use of the [DKPro Core Type System (current v1.9.0)](https://dkpro.github.io/dkpro-core/releases/1.9.0/docs/typesystem-reference.html) for known types shared between the components; this typesystem is already available at Maven. For types not covered by the DKPro Core Type System, users can select a typesystem of their choice, document it following the specifications for ancillary knowledge resources and upload it at Maven.
[^2]: You can find examples of OMTD-SHARE metadata records [here](https://openminted.github.io/releases/omtd-share/3.0.2/).

