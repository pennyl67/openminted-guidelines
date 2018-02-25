##Providers of corpora
Content may be imported in OpenMinTeD in the form of [single documents](/guidelines_for_providers_of_publications/README.md) or already packaged in the form of **corpora**, i.e. collections of single documents. 

Corpora may come (upon bilateral agreements) from repositories of language resources, or discipline-specific repositories, or **uploaded by users** for processing with TDM applications.

If you wish to share corpora through OpenMinTeD, you will find more information [here](/guidelines_for_providers_of_corpora/instructions_for_providers_of_corpora.md).

##What types of corpora
Corpora in the OpenMinTeD framework refer mainly to _**collections of documents that will be used as mining source**_ in the TDM process. If they are uploaded in OpenMinTeD, they may not necessarily be composed of scholarly works. Examples include reference corpora \(i.e. corpora deemed representative of general language or a sublanguage usage\), news corpora, collections of domain-specific texts, such as manuals, technical reports, etc., as well as annotated corpora, such as treebanks, morphologically tagged golden corpora etc. Nevertheless, in order to be mined they must follow the technical requirements that have been defined for corpora built through the OpenMinTeD mechanism[^1].
Otherwise, they can be used \(**upon availability of the respective components/applications**\) for other objectives, such as training Machine Learning models, evaluating the performance of applications, etc.

{% blurb style='warning'%}
At present, OpenMinTeD processes only **raw corpora** that follow all the technical specifications defined for corpora built through the OpenMinTeD mechanism.
{% endblurb %}

###Minimum requirements for corpora
If you want to share your corpus through OpenMinTeD, you must
* ensure that the single documents comprising the corpus adhere to the minimal level of the [OpenMinTed Interoperability specifications](/guidelines_for_providers_of_publications/recommendations-for-publishers.md), 
* describe the corpus with a metadata record compliant with the [OMTD-SHARE schema](/guidelines_for_providers_of_corpora/recommended_schema_for_corpora.md), at least at the minimal level,
* prepare, package and register a zipped file with the contents (texts) of the corpus according to the [instructions for uploading corpora](/guidelines_for_providers_of_corpora/instructions_for_providers_of_corpora.md).

---
[^1]: In the case of single documents (publications) uploaded in the registry, the OpenMinTeD platform includes a mechanism for automatically generating corpora based on user criteria selected from a faceted view - more details are included in the [Building corpora of scholarly content offered in OpenMinTeD](/deployment-scenario-of-publications-in-openminted.md).

