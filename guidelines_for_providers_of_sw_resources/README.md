# ​Guidelines for providers of software \(applications and components\) {#guidelines-for-providers-of-s-w-resources}

We welcome 
* end-user **applications **that can be used as-is to perform TDM operations on content resources, as well as
* **components**, i.e. pieces of software that perform basic tasks; using the OpenMinTeD Workflow Editor, TDM developers can combine together components and tune them with ancillary knowledge resources in order to build applications that will be offered to end-users.

![](/assets/4a.png)

If you wish to share TDM software through the [OpenMinTeD platform](https://services.openminted.eu/home), you must

* provide access to an **executable **of the software in one of the ways specified in the next sections, 

* add the software in the [OpenMinTeD registry](https://services.openminted.eu/resourceRegistration/component) with a **metadata record **compliant with the  [OMTD-SHARE schema](/guidelines_for_providers_of_sw_resources/recommended_schema_for_sw_resources.md), at least at the minimal level

* adhere to the [OpenMinTeD interoperability specifications](/guidelines_for_providers_of_sw_resources/how-to-make-your-components-interoperable.md), ensuring at least that your softoare supports \(i.e. produces & consumes\) **data in the [XML Metadata Interchange \(XMI\)](http://www.omg.org/spec/XMI/) format**[^1]; if not, you should provide appropriate readers and writers for converting XMI messages from and to the components’ format.

---

[^1]: As also happens in the UIMA framework.

