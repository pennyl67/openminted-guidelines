### Sharing apps/components as Docker images

Software \(apps/components\) from frameworks and technologies other than UIMA and GATE must be registered in OpenMinTeD as [Docker](https://docs.docker.com) images.

#### **Step 1 - Preparing and packaging**

To build an OpenMinTeD-compatible Docker image of apps/components, you must follow the specifications described at [https://openminted.github.io/releases/docker-spec/0.1.0/specification](https://openminted.github.io/releases/docker-spec/0.1.0/specification) and upload it to the [Docker hub](https://hub.docker.com/).

#### **Step 2 - Registering in OpenMinTeD**

You can then visit the [OpenMinTeD registry](https://services.openminted.eu) where you can register your app/component in one of the following ways:

* edit from scratch the OMTD-SHARE metadata record[^1] using the OpenMinTeD editor or

* upload an XML file with the OMTD-SHARE metadata record

In both cases, the metadata record can be viewed and edited at the end of the process.

The location of the docker image must be provided in the element &lt;distributionLocation&gt; while the identifier of the app/component that is inside the docker image must be encoded in the element &lt;resourceIdentifier&gt;, e.g.

`<distributionLocation>bibliome/alvisengine</distributionLocation>`

`<resourceIdentifier resourceIdentifierShemeName="omtd-docker">org.bibliome.alvisnlp.modules.ccg.CCGParser</resourceIdentifier>`

Further requirements and recommendations for achieving interoperability across software and content resources are presented [here](/guidelines_for_providers_of_sw_resources/how-to-make-your-components-interoperable.md).

[^1]: You can find example metadata records [here](/guidelines_for_providers_of_sw_resources/examples-for-software-resources.md).

