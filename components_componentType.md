#### componentType
##### Usage
Mandatory
##### Type
open controlled vocabulary
##### Controlled vocabulary reference and/or values
ms-omtd:componentType: _access_, _reader_, _writer_, _supportComponent_, _visualizer_, _debugger_, _validator_, _viewer_, _corpusViewer_, _lexiconViewer_, _editor_, _mlTrainer_, _mlPredictor_, _featureExtractor_, _dataSplitter_, _dataMerger_, _converter_, _evaluator_, _flowController_, _scriptBasedAnalyzer_, _matcher_, _gazetteerBasedComponent_, _crowdSourcingComponent_, _dataCollector_, _crawler_, _processingComponent_, _annotator_, _segmenter_, _stemmer_, _lemmatizer_, _tagger_, _chunker_, _parser_, _coreferenceAnnotator_, _namedEntityRecognizer_, _semanticsAnnotator_, _srlAnnotator_, _readabilityAnnotator_, _aligner_, _generator_, _summarizer_, _simplifier_, _naturalLanguageGenerator_, _prePostProcessor_, _spellingChecker_, _grammarChecker_, _normalizer_, _filters_, _extractor_, _topicExtractor_, _documentClassifier_, _languageIdentifier_, _sentimentAnalyzer_, _keywordsExtractor_, _terminologyExtractor_, _contradictionDetector_, _emotionRecognizer_, _eventExtractor_, _persuasiveExpressionMiner_, _informationExtractor_, _lexiconExtractorFromCorpora_, _lexiconExtractorFromLexica_, _wordSenseDisambiguator_, _qualitativeAnalyser_
##### Definition/Explanations
Specifies the type of the component in terms of the function/task it performs
##### Recommended usage
Please, select one of the predefined values. It should be noted that the values are hierarchically organised, so it's recommended to select the more specific value applicable (e.g. "visualizer" rather than the broader "supportComponent").  
The current list of values is intended for use mainly by simple components rather than workflows or full applications. The list will be further enriched with values that target the end-users also.
##### Relation to other metadata schema elements
* **DCMI:** skos:narrowMatch dct:type
