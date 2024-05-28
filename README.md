# NLP_translation
Integration of Coreference Resolution into Machine Translation from Non-gendered to Gendered Languages

Final project for MIT's Quantitative Methods for Natural Language Processing class (6.8610), Fall 2022

## Description
We integrated a coreference resolution system with a transformer machine translation system to improve gender agreements between pronouns/nouns and adjectives in translations
from non-gendered to gendered languages.

## Instructions
This repository contains all of the code files for our project. Each notebook contains the code we ran for a certain language and approach combination.

The files are:

* ```CLR_Irish_0_Baseline_Model.ipynb```: contains the Irish baseline model
* ```CLR_Spanish_0_Baseline_Model.ipynb```: contains the Spanish baseline model
* ```CLR_Spanish_1_Coreference_Resolution.ipynb```: contains the Spanish model with coreference information added
* ```CLR_Spanish_2_Adjective_Reference.ipynb```: contains the Spanish model with coreference resolution and adjective reference information added
* ```CLR_Spanish_3_Gender_Balancing_Dataset.ipynb```: contains the Spanish model with coreference resolution and adjective reference information added, but with a gender balanced dataset.

Instructions for running each model are included in the script. For most notebooks, this requires running each cell in sequential order.

To access the necessary data for each notebook, please see the following:

**For ```CLR_Spanish_0_Baseline_Model.ipynb```, ```CLR_Spanish_1_Coreference_Resolution.ipynb```, and ```CLR_Spanish_2_Adjective_Reference.ipynb```:**

The Spanish dataset necessary for these notebooks are hosted on the internet in an open access manner. The notebooks already contain code cells that load and pre-process the dataset.

**For  ```CLR_Irish_0_Baseline_Model.ipynb```:**

The Irish dataset is included in the file ```en-ga.txt```. To use the file, please save and upload the dataset into your Google Drive. When running the Google Colab notebook, please change the file path to the dataset text file accordingly.

**For  ```CLR_Spanish_3_Gender_Balancing_Dataset.ipynb```:**

The additional books dataset (translated between Spanish and English) is included in the folder. There are two files, ```book-en-sentences.txt``` and ```book-es-sentences.txt```, containing the sentences in English and the corresponding Spanish translations respectively. Each new line in the ```book-en-sentences.txt``` corresponds to a line in the ```book-es-sentences.txt``` file. To use the file, please save and upload the dataset into your Google Drive. When running the Google Colab notebook, please change the file path to the dataset text file accordingly.
