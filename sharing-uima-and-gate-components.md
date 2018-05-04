### How to share UIMA and GATE components through MAVEN

You can provide components compatible with the [UIMA](https://uima.apache.org/)[^1] and [GATE](https://gate.ac.uk/) frameworks through the [Maven Central repository](https://mvnrepository.com/) according to the following instructions. Components provided in this mode are dockerized by OpenMinTeD.[^2]

{% blurb style='warning'%}
**Don't forget!** Check that your software complies with **at least the minimal level** of the [OpenMinTeD interoperability requirements and recommendations](/guidelines_for_providers_of_sw_resources/how-to-make-your-components-interoperable.md).
{% endblurb %}

#### **Step 1 - Preparing and packaging**

* Please, put together in a single folder \(in the form that is required by the used technologies/frameworks\)
  * all files that implement the component \(e.g. Java classes, etc.\)
  * licence text\(s\), preferably in a text file entitled "LICENCE.TXT" in order to be unambiguously recognised; in the case of multiple licences, they should be all aggregated in the same file
  * a "readme" notice, that describes the contents of the folder as well as any important notice for the compilation and execution of the component
  * all descriptors \(UIMA/uimaFIT, GATE CREOLE, OMTD-SHARE etc.\) available for the component according to the implementation framework[^3]
  * a "descriptors.txt" file in the folder META-INF/eu.openminted.share with a list of the descriptors
  * a Maven POM XML file.
* Pack them as a JAR using the respective Maven plugin.
* Upload them to the Maven repository according to the [Maven guidelines](http://maven.apache.org/guides/mini/guide-central-repository-upload.html).

{% blurb style='tip'%}
Please, make sure that you add the following elements in the POM: _name_, _description_, _version_, _organization URL_ (for developers) and _license name_. These are needed for creating a valid OMTD-SHARE metadata record.
{% endblurb %}

#### **Step 2 - Adding in the OpenMinTeD platform**

You can then visit the [OpenMinTeD registry](https://services.openminted.eu/resourceRegistration/component) where you can register your component in one of the following ways:

* create from scratch the OMTD-SHARE metadata record \(minimal schema\) using the OpenMinTeD editor; in this case, you must specify the Maven coordinates in the metadata element _**distributionLocation**_, e.g. `<distributionLocation>mvn:de.tudarmstadt.ukp.dkpro.core:de.tudarmstadt.ukp.dkpro.core.berkeleyparser-gpl:1.9.0#de.tudarmstadt.ukp.dkpro.core.berkeleyparser.BerkeleyParser</distributionLocation>`
* upload the OMTD-SHARE metadata record[^4] as an XML file with the Maven coordinates filled in the relevant metadata element as in the above example, or
* submit the Maven coordinates directly in the interface; in this case, 
  * if the package includes one or more  OMTD-SHARE files corresponding to the components contained in the package, the available components will be displayed to the user, the user will select the component to register, the metadata will be validated and, if valid, uploaded to the registry; 
  * if there are no OMTD-SHARE files in the package, an OMTD-SHARE record can be partially converted from the Maven POM file and other descriptors and the user will be prompted to fill in the missing information.

In all of these cases, the metadata record can be viewed and edited at the end of the process.

---

[^1]: Please note that the OpenMinTeD UIMA wrapper is presently only compatible with UIMA components using UIMA version 2.8.1 or higher. Older versions of UIMA 2.x might work as well, but there is no guarantee. UIMA 3.x is presently not supported. This applies only to UIMA components submitted via Maven. Components using Docker are not affected and may internally make use of any UIMA version.
[^2]: If you prefer, you can provide your components as Docker images following the  relevant [instructions](https://guidelines.openminted.eu/sharing-components-as-dockerised-images.html). 
[^3]: You will find more information on how to embed the OMTD-SHARE metadata records in the package and how to use related tooling [here](https://builds.openminted.eu/view/WP%205.2/job/OpenMinTeD%20SHARE%20Annotations/eu.openminted.share.annotations%24omtd-share-annotations-doc/doclinks/1/#sect_introduction).
[^4]: You can find examples of OMTD-SHARE metadata records [here](https://openminted.github.io/releases/omtd-share/3.0.2/).

