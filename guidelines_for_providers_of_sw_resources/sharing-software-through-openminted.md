## How to share software \(applications and components\)

We welcome software in the [OpenMinTeD platform](https://services.openminted.eu/resourceRegistration/component)

* fully packaged as an end-user application or 
* as separate components, offering the advantage that it can be re-used in the creation of new applications.

In addition, in order to overcome hurdles associated with platform dependent implementations, OpenMinTeD recommends the use of **Docker images**[^1]. For components compatible with specific frameworks, dockerization is undertaken by OpenMinTeD.


There are three ways you can add TDM software in OpenMinTeD:

* [**components compatible with UIMA**[^2]** or GATE**[^3]** frameworks**](//sharing-uima-and-gate-components.md)** **can be uploaded in the [Maven Central repository](http://maven.apache.org) and registered by declaring the respective Maven coordinates which uniquely specify their  location; dockerization for these components is undertaken by OpenMinTeD;
* [**components or applications created with other technologies or other TDM-related frameworks**](//sharing-components-as-dockerised-images.md)** **must be packaged  and registered directly as Docker images;
* [**web services**](//guidelines_for_providers_of_sw_resources/sharing-web-services.md) \(applications/components\) which are installed and maintained outside the OpenMinTeD platform must be registered with the URL that specifies their location. The client that communicates with the web service is implemented by OpenMinTeD.


In both cases, it must be deposited as explained in the following sections, at **specific repositories **following technical procedures and specifications that ensure it can be accessed at any time and executed as expected. When invoked for execution in the [OpenMinTeD platform](https://services.openminted.eu/runApplication), the software is retrieved from these repositories in order to be deployed.

In addition, in order to overcome hurdles associated with platform dependent implementations, OpenMinTeD recommends the use of **Docker images**[^1]. For components compatible with specific frameworks, dockerization is undertaken by OpenMinTeD.

Alternatively, TDM developers can also expose their software through the **Processing Web Service API layer** that has been specified by OpenMinTeD.


---

[^1]: Docker is a middleware technology that packages software along with their dependencies in order to run independently of operating systems or local setup - see more at [https://docs.docker.com](https://docs.docker.com).

[^2]: For more information, see [https://uima.apache.org/](https://uima.apache.org/).

[^3]: For more information, see [https://gate.ac.uk/.](https://gate.ac.uk/)

