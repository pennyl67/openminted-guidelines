#### componentDependencies

##### Usage

Mandatory when applicable

##### Type

set of elements

##### Mandatory and recommended elements

| **Element** | **Usage** | **Type** |
| :--- | :--- | :--- |
| typesystem | Mandatory when applicable | resourceName & optional resourceIdentifier |
| annotationSchema | Mandatory when applicable | resourceName & optional resourceIdentifier |
| annotationResource | Mandatory when applicable | resourceName & optional resourceIdentifier |
| mlModel | Mandatory when applicable | resourceName & optional resourceIdentifier |

##### Definition/Explanations

Specifies the dependencies \(language resources\) of the application/component; the recommended way is to specify the resourceName and \(optionally\) the resourceIdentifier of the relevant resource.

* **typesystem**:  A set of elements designed to annotate data. It typically contains only a list of annotation types, i.e. specific labels that are used for the annotation \(e.g. part-of-speech, person, organization, etc.\), and is usually inbuilt in the annotation software.
* **annotationSchema**:  A set of elements and values designed to annotate data. It usually consists in a formal representation. It aims to represent a specific level of information, such as morphological features of words, syntactic dependency relations between phrases, discourse level information etc. It can consist of a flat structure of elements and values \(e.g. part-of-speech tags\) or it can be more complex with interrelated elements \(e.g. specific morphological features to be used for each part-of-speech\)
* **annotationResource**: Any resource that can be used for annotating a document or corpus, e.g. an ontology, a lexicon, a list of named entities etc.

* **mlModel**: The model artifact that is created through a training process involving an ML algorithm \(that is, the learning algorithm\) and the training data to learn from.





