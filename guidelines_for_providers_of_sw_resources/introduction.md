## Introduction {#introduction}

OpenMinTeD targets scholarly researchers who are agnostic to s/w details and peculiarities as well as TDM developers. It allows, therefore, the registration of

*   applications, that can be used as-is to perform TDM operations on content resources, and
*   s/w components, i.e. pieces of s/w that can, by means of the OpenMinTeD Workflow Editor, be put together and tuned with various ancillary resources in order to create workflows that will be delivered to the end-users and/or further integrated into other workflows.

All of these will be made available to the researchers in a way that will not require any kind of expertise from them, both as locally downloadable and executable tools or as web services.

The OpenMinTeD platform, at the current stage, supports the integration of

*   web services as Docker images, or
*   s/w components wrapped for the GATE or UIMA/uimaFIT frameworks.

To be fully compatible with OpenMinTeD, you must provide

*   a metadata record compliant with the OMTD-SHARE schema, at least at the minimal level (which you can upload to the Registry as an XML file and/or edit with the OpenMinTeD metadata editor),
*   the s/w in an executable form, by uploading it in a compressed file or providing a link to a URL location from which it can be directly accessed (i.e. not a landing page).