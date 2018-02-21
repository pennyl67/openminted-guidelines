## How to share software \(applications and components\)

You can share your TDM software through the [OpenMinTeD platform](https://services.openminted.eu/resourceRegistration/component)

* fully packaged as an end-user **application **or 
* as separate **components**, offering the advantage that it can be re-used in the creation of new applications.

For both of these and in order to overcome hurdles associated with platform dependent implementations, we accept software executables in the form of **Docker images**[^1] or **web services** that follow technical procedures and specifications set by OpenMinTeD. These specifications ensure that the software can be accessed at any time and executed as expected. 

![](/assets/4a.png)

There are three ways you can add TDM software in the [OpenMinTeD platform](https://services.openminted.eu/home):
* **components compatible with UIMA[^2] or GATE[^3] frameworks**: prepare, upload in the [Maven Central repository](http://maven.apache.org) and register them according to the [instructions](//sharing-uima-and-gate-components.md); dockerization for these components is undertaken by OpenMinTeD;
* **components or applications created with other technologies or other TDM-related frameworks**: prepare, package and register directly as Docker images according to the instructions described [here](//sharing-components-as-dockerised-images.md);
* [**web services**](//guidelines_for_providers_of_sw_resources/sharing-web-services.md) \(applications/components\): if you want to maintain your software outside the OpenMinTeD platform, you must expose it through the **Processing Web Service API layer** that has been specified by OpenMinTeD and register it according to the instructions described [here](//guidelines_for_providers_of_sw_resources/sharing-web-services.md); the client that communicates with the web service is implemented by OpenMinTeD.


---

[^1]: Docker is a middleware technology that packages software along with their dependencies in order to run independently of operating systems or local setup - see more at [https://docs.docker.com](https://docs.docker.com).

[^2]: For more information, see [https://uima.apache.org/](https://uima.apache.org/).

[^3]: For more information, see [https://gate.ac.uk/.](https://gate.ac.uk/)

