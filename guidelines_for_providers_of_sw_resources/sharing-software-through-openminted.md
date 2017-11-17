

## Sharing software \(applications and components\)

Software can be registered in OpenMinTeD 

* fully packaged as an end-user application or 
* as separate components, offering the advantage that they can be re-used in the creation of new applications.

In both cases, it should be deposited at **specific repositories **following technical procedures and specifications that ensure it can be accessed at any time and executed as expected. When invoked for execution in the OpenMinTeD platform, the software is retrieved from these repositories in order to be deployed.

In addition, in order to overcome hurdles associated with platform dependent implementations, OpenMinTeD recommends the use of **Docker images**[^1]. For components compatible with specific frameworks, dockerization is undertaken by OpenMinTeD.

Alternatively, TDM developers can also expose their software through the **Processing Web Service API layer** that has been specified by OpenMinTeD.

There are, therefore, three ways you can provide TDM software in OpenMinTeD:

* **components compatible with UIMA or GATE frameworks **can be uploaded in the [Maven Central repository](http://maven.apache.org) and registered by declaring the respective Maven coordinates which uniquely specify their  location; dockerization for these components is undertaken by OpenMinTeD;
* **components created with other technologies or other TDM-related frameworks **must be packaged  and registered directly as Docker images;
* **web services** which are installed and maintained outside the OpenMinTeD platform are accessed via an appropriate client following the OpenMinTeD specifications; they must be registered in OpenMinTeD with the URL that specifies their location.

---

[^1]: Docker is a middleware technology that packages software along with their dependencies in order to run independently of operating systems or local setup - see more at [https://docs.docker.com](https://docs.docker.com).

