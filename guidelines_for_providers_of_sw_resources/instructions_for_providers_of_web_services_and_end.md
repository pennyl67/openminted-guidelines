## ​Instructions for providers of web services and end-user applications {#instructions-for-providers-of-web-services-and-end-user-applications}

### Packaging and uploading procedures {#packaging-and-uploading-procedures}

S/w resources can be uploaded by registered users as decided in the OpenMinTeD Policies.

The recommended way of providing **_web services_ **is through Docker repositories according to the following instructions:

*   Submit the appropriate URL link or image id.

### Technical requirements {#technical-requirements}

In addition, if you want to be fully compliant with the OpenMinTeD interoperability requirements, please ensure that you adopt the following rules; if you fail to abide to them, it might still be possible to operate your s/w resources via the OpenMinTeD platform, but this cannot be guaranteed and interoperability with other resources will suffer loss.

In addition, when OpenMinTeD web services are hosted on GRNET&#039;s cloud service, they are limited by the ~okeanos resource management contemporaneous constraints and policies, i.e. each service being deployed at a Docker-enabled VM:

*   can only run on a ~okeanos-supported host operating system, more information here: [https://okeanos.grnet.gr/support/faq/okeanos-what-operating-systems-are-available-to-install-on-my-vms/](https://okeanos.grnet.gr/support/faq/okeanos-what-operating-systems-are-available-to-install-on-my-vms/)
*   cannot surpass the CPU/Cores/Disk limit imposed by ~okeanos and by the ~okeanos OMTD project in total.

### ****Documentation/Metadata requirements**** {#documentation-metadata-requirements}

To be fully compatible with OpenMinTeD, you must

*   ensure that the s/w is distributed under a perpetual, world-wide, no-charge, royalty-free copyright/patent license that permits unrestricted use and allows unlimited redistribution
*   include in the metadata record a link to the licence document(s) with the terms and conditions under which it is provided, and attach the licence document(s) together with the resource
*   if you already have a PID for your resource (e.g. a URI or a HANDLE), make sure it is included in the metadata record
*   ensure that you version all your s/w resources and label the versions in an unambiguous way, preferably following the Semantic Versioning recommendations[^36].

Further recommendations that contribute to interoperability include the following:

*   It is important that you provide the appropriate documentation for your resource (e.g. manuals, help files etc.), which you should also version along with the s/w and add as reference to your metadata record.
*   Describe all the executional requirements for the proper operation of the s/w, i.e. required s/w libraries, ancillary resources, annotation schema dependencies etc.
*   Describe the input and output requirements for your s/w, at least as regards the type of resource, the language (if required), data format and character encoding, and annotation types of the input/output resource.
*   Declare that the s/w can only be accessed as a web service in the metadata.
*   Ensure that you describe appropriately the functionalities of the s/w, both through the OMTD-SHARE component type vocabulary (pending link) as well as in a free text description, supplying more information for the user.
*   In all cases, where linking to other resources or entities (e.g. persons, projects etc.), please try to do this through unique and persistent identifiers of authority lists and sources, to the extent possible, documenting also the authority and/or scheme it adheres to.

[^36]: