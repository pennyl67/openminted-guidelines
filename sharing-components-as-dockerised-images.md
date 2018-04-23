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

* upload an XML file with the OMTD-SHARE metadata record.

In both cases, the metadata record can be viewed and edited at the end of the process.

{% blurb style='warning'%}
**Important: the following elements must be in the metadata record as described below, otherwise the app/component will not run!** 


* OpenMinTeD looks into the Central Docker hub to locate the docker images; so, please provide in the element **_distributionLocation_** (a) the docker image name and (b) the version; i.e. OpenMinTeD will use the command "docker pull _image_name:version_" to retrieve the image, so in the _**distributionLocation**_ you must add _image_name:version_

    `<distributionLocation>bibliome/alvisengine:1.0.0</distributionLocation>`


* Please add the command for invoking the app/component in the metadata element _**command**_, e.g.

    `<command>alvisnlp org.bibliome.alvisnlp.modules.ccg.CCGParser</command>`

The _**command **_element must (a) only contain your executor i.e. the part required to run your command by excluding the parameters and their respective values, and (b) be available to run from everywhere in the docker image (i.e. add your executor in the /usr/bin/ or use absolute paths).

{% endblurb %}



---


[^1]: You can find examples of OMTD-SHARE metadata records [here](https://openminted.github.io/releases/omtd-share/3.0.2/).

