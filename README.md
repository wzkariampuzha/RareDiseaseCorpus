# RareDiseaseCorpus
This project generates a corpus of 7699 rare disease abstracts. 

## LTSM RNN Classifier
### Key notebooks
- *gather_pubs_per_disease.ipynb*: Queries the [EBI RESTful API](https://www.ebi.ac.uk/ebisearch/apidoc.ebi) for 500 disease names and synonyms and retrieves abstracts until at least 50 abstracts returned or results exhausted and saves results in *whole_abstract_set.csv*. Although ~25,000 abstracts were expected, 7699 unique abstracts were returned on 488 diseases due to limited research on rare diseases.
- *csv2txtfolder.ipynb*: Converts the saved abstracts into a folder of text files which comprises the corpus.

### Data files
- *GARD.csv*: List of rare disease names and synonyms from the [NIH Genetic and Rare Disease Information Center](https://rarediseases.info.nih.gov/)
- *whole_abstract_set.csv*: Contains 7699 unique abstracts (9284 total) that were returned from the EBI API call.

### Top 50 Lemmas
| Rank | Frequency | Lemma     |
|------|-----------|-----------|
| 1    | 70745     | the       |
| 2    | 62091     | of        |
| 3    | 58537     | and       |
| 4    | 42279     | be        |
| 5    | 41340     | in        |
| 6    | 30050     | a         |
| 7    | 26552     | to        |
| 8    | 24907     | with      |
| 9    | 19775     | h         |
| 10   | 14487     | patient   |
| 11   | 12525     | for       |
| 12   | 10903     | we        |
| 13   | 9624      | i         |
| 14   | 9498      | have      |
| 15   | 8445      | that      |
| 16   | 8248      | by        |
| 17   | 7944      | as        |
| 18   | 7547      | this      |
| 19   | 6357      | or        |
| 20   | 6338      | on        |
| 21   | 6221      | ares      |
| 22   | 6076      | study     |
| 23   | 5874      | disease   |
| 24   | 5733      | an        |
| 25   | 5458      | from      |
| 26   | 5206      | case      |
| 27   | 4992      | p         |
| 28   | 4882      | result    |
| 29   | 4491      | syndrome  |
| 30   | 4482      | clinical  |
| 31   | 4455      | diagnosis |
| 32   | 4389      | gene      |
| 33   | 4363      | use       |
| 34   | 4349      | at        |
| 35   | 4059      | cell      |
| 36   | 4013      | report    |
| 37   | 3991      | mutation  |
| 38   | 3801      | year      |
| 39   | 3669      | include   |
| 40   | 3580      | treatment |
| 41   | 3527      | present   |
| 42   | 3510      | disorder  |
| 43   | 3501      | associate |
| 44   | 3482      | it        |
| 45   | 3446      | find      |
| 46   | 3419      | these     |
| 47   | 3410      | which     |
| 48   | 3271      | c         |
| 49   | 3074      | group     |
| 50   | 3069      | not       |
