### How to share apps/components as Docker images

Software \(apps/components\) from frameworks and technologies other than UIMA and GATE must be registered in OpenMinTeD as [Docker](https://docs.docker.com) images.

{% blurb style='warning'%}
**Don't forget!** Check that your software complies with **at least the minimal level** of the [OpenMinTeD interoperability requirements and recommendations](/guidelines_for_providers_of_sw_resources/how-to-make-your-components-interoperable.md).
{% endblurb %}


#### **Step 1 - Preparing and packaging**

To build an OpenMinTeD-compatible Docker image of apps/components, in addition to the Docker guidelines, you must follow the relevant [OpenMinTeD specifications for dockerized components](https://openminted.github.io/releases/docker-spec) and upload it to the [Docker hub](https://hub.docker.com/).

#### **Step 2 - Adding in the OpenMinTeD platform**

You can then visit the [OpenMinTeD registry](https://services.openminted.eu) where you can register your app/component in one of the following ways:

* edit from scratch the OMTD-SHARE metadata record[^1] using the OpenMinTeD editor or

* upload an XML file with the OMTD-SHARE metadata record

In both cases, the metadata record can be viewed and edited at the end of the process.

The location of the docker image must be provided in the element **_distributionLocation_**; and the command for invoking the app/component (toghether with the id of the app/component) in the element _**command**_, e.g.
    `<distributionLocation>bibliome/alvisengine</distributionLocation>`
`<command>alvisnlp org.bibliome.alvisnlp.modules.ccg.CCGParser</command>`




[^1]: You can find example metadata records [here](/guidelines_for_providers_of_sw_resources/examples-for-software-resources.md).

