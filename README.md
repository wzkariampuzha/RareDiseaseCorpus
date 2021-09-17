# RareDiseaseCorpus
This project is a corpus of 7699 rare disease abstracts. 


an in-progress alert system for the [NIH Genetic and Rare Diseases Information Center (GARD)](https://rarediseases.info.nih.gov/). The purpose of this system is to automatically 


### Data files
- *whole_abstract_set.csv*: Contains 7699 unique abstracts (9284 total) that were returned from the EBI API call.

## LTSM RNN Classifier
### Key notebooks
- *gather_pubs_per_disease.ipynb*: Queries the [EBI RESTful API](https://www.ebi.ac.uk/ebisearch/apidoc.ebi) for Generates *whole_abstract_set* and *positive_abstract_set.csv*. *whole_abstract_set* is a dataset created by sampling 500 rare disease names and their synonyms from *GARD.csv* until &ge;50 abstracts had been returned or the search results were exhausted. Although ~25,000 abstracts were expected, 7699 unique abstracts were returned due to the limited research on rare diseases.
- *Analyze_dz_num_sample.ipynb*: Combines

### Data files
- *GARD.csv*: List of rare disease names and synonyms from the [NIH Genetic and Rare Disease Information Center](https://rarediseases.info.nih.gov/)
- *whole_abstract_set.csv*: Contains 7699 unique abstracts (9284 total) that were returned from the EBI API call.
