## CLOD

Changes to the ontology:

* TODO: LR to fix the provenance generated to link the metricCalculation activity to the laundromat dataset
* Added rdfs:isDefinedBy links from everything defined in the ontologies to the respective ontology URI
* Corrected import structure (every use of an external namespace is accompanied by a proper owl:imports statement)
* Corrected VANN and VOAF attributes of ontology definitions.
* Added VOAF specializes (VOID), generalizes (VOID-Ext) to metrics ontology
* Corrected several inconsistent namespace declarations and uses across all ontology files (httpo, metrics, error, ontology)
* Replaced author blank nodes with actual foaf:Person URIs
* Corrected property and class types across datasets (datatype properties vs. object properties, owl:Class vs rdfs:Class)
* Added mappings to PROV plans and entities, corrected link between prov:Activity of metrics generation and the dataset used. 
* Added mappings to VOID Dataset, and from llm:IRIs, llm:definedClasses and llm:definedProperties to void:entities, void:classes and void:properties, respectively.
* Added mappings to VOID-ext, llm:literals and llm:blankNodes generalize void-ext:distinctLiterals and void-ext:distinctBlankNodes, respectively
* Used property chain axioms to relate property chains such as llm:IRILength->llm:mean with void-ext:averageIRILength.
