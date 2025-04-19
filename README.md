# Bert-Driven-Equalizer

This project explores a semantic-driven equalizer powered by BERT. It allows users to describe EQ settings in natural language and hear the corresponding changes in audio.  
And it's not finished yet.

## 🔍 Baseline Research
Part of this project and codes are based on the research by Venkatesh et al. (2022), which explores using word embeddings for automatic equalization in audio mixing.  
You can read the original paper: [*Word Embeddings for Automatic Equalization in Audio Mixing*](https://arxiv.org/abs/2202.08898).
## 🔧 Files

- [Play_and_Listen.ipynb](./Play_and_Listen.ipynb): Try and listen, looking into the performance of the model.
- [ModelTraining&Testing.ipynb](./ModelTraining&Testing.ipynb): Contains training and evaluation code for the model.
- [Embedding-extraction.ipynb](./Embedding-extraction20%copy.ipynb): Embedding extraction method from Bert model.
- [data-preprocess.ipynb](./data-preprocess20%copy.ipynb): Preprocessing and looking into the SocialEQ Dataset.
- [e_gtr_short.wav](./e_gtr_short.wav): Sample guitar audiofile for testing.

## 📄 SocialEQ Dataset
- You can get the SocialEQ dataset from [here](https://www.dropbox.com/scl/fo/ulk8t7ad5b1js8qwuph3f/ANnatQNiD1QoQoeDDZktHjM/data/raw?e=1&preview=eq_contributions.csv&rlkey=we20hw9qu94wytocopw5np1yj&subfolder_nav_tracking=1&dl=0).

## ▶️ Usage
Open the [Play_and_Listen.ipynb](./Play_and_Listen.ipynb) and follow the instructions to try the model with audio.
  
