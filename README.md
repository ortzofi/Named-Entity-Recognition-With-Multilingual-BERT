# Named Entity Recognition With Multilingual BERT
## About 
As part of a deep learning course at Reichman University (IDC Herzliya) we chose to take on an NLP (Natural Language Processing) final project. The project’s goal was to check how source languages affect the performance of Multilingual BERT in cross-lingual zero-shot named entity recognition (NER) prediction. Annotated data in 17 different languages and 9 NER tags were obtained for this purpose. For more details please refer to the paper included in this repository.

## Process
The process included building 10 different Multilingual BERT models, each fine-tuned for NER and trained on different languages: three models were trained on one language, four models were trained jointly on two languages, and three models were trained jointly on three languages. Then, each model was evaluated on 17 languages, some of which do not share the same script and structure, with zero-shot inference. Performance was measured by F1 score. 

## Data and Languages
We used the English CoNLL 2003 dataset as well as the Spanish and Dutch CoNLL 2002 dataset which are widely used in NER research. We also used the German GermEval 2014 dataset, the Danish DaNE dataset and the Afrikaans NER Corpus developed by North-West University, South Africa. All these datasets use the CoNLL annotation standards and have four entity types (PER, LOC, ORG, MISC).
In addition, we used the Chinese MSRA dataset and the WikiANN dataset, from which we took the French, Italian, Portuguese, Swedish, Turkish, Russian, Hebrew, Arabic, Japanese and Korean datasets. These datasets have three entity types (PER, LOC, ORG).

## Results
This table displayes the F1 score achieved by each model on the target languages, including the total average score.
<img width="1001" alt="Screen Shot 2022-01-08 at 13 44 56" src="https://user-images.githubusercontent.com/96059174/148642882-21d6d3e7-3ed7-47ba-ae8d-aaa42c673aac.png">

In this example we can see the full results of a model trained on English and Spanish and evaluated on Spanish data.
<img width="417" alt="Screen Shot 2022-01-08 at 14 15 01" src="https://user-images.githubusercontent.com/96059174/148643775-c9c46b2b-275a-4939-92df-862d406e83f2.png">
