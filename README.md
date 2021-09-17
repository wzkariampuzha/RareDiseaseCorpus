# RareDiseaseCorpus
This project is a corpus of 7699 rare disease abstracts. 

## LTSM RNN Classifier
### Key notebooks
- *gather_pubs_per_disease.ipynb*: Queries the [EBI RESTful API](https://www.ebi.ac.uk/ebisearch/apidoc.ebi) for 500 disease names and synonyms and retrieves abstracts until at least 50 abstracts returned or results exhausted and saves results in *whole_abstract_set.csv*. Although ~25,000 abstracts were expected, 7699 unique abstracts were returned due to limited research on rare diseases.
- *Analyze_dz_num_sample.ipynb*: Analyzes distribution of the *whole_abstract_set*.
- *csv2txtfolder.ipynb*: Converts the saved abstracts into a folder of text files which comprises the corpus.

### Data files
- *GARD.csv*: List of rare disease names and synonyms from the [NIH Genetic and Rare Disease Information Center](https://rarediseases.info.nih.gov/)
- *whole_abstract_set.csv*: Contains 7699 unique abstracts (9284 total) that were returned from the EBI API call.
