### Sharing components as Docker images

Components from frameworks and technologies other than UIMA and GATE must be registered in OpenMinTeD as Docker images.

#### **Step 1 - Preparing and packaging**

To build an OpenMinTeD-compatible Docker image of components, you must follow the specifications described at [https://openminted.github.io/releases/docker-spec/0.1.0/specification](https://openminted.github.io/releases/docker-spec/0.1.0/specification) and upload it to the [Docker hub](https://hub.docker.com/).

#### **Step 2 - Registering in OpenMinTeD**

You can then visit the OpenMinTeD registry where you can register your component in one of the following ways:

* edit from scratch the OMTD-SHARE metadata record using the OpenMinTeD editor or

* upload an XML file with the OMTD-SHARE metadata record

In both cases, the metadata record can be viewed and edited at the end of the process.

The location and identifier of the component must be provided in the elements &lt;distributionLocation&gt; and &lt;resourceIdentifier&gt;, e.g.

`<distributionLocation>bibliome/alvisengine</distributionLocation>`

`<resourceIdentifier resourceIdentifierShemeName="omtd-docker">org.bibliome.alvisnlp.modules.ccg.CCGParser</resourceIdentifier>`

Further requirements and recommendations for achieving interoperability across components and with the content resources are presented [here](/guidelines_for_providers_of_sw_resources/how-to-make-your-components-interoperable.md).

