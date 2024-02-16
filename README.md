# Sentiment Analysis on Movie Reviews
Classify the sentiment of sentences from the Rotten Tomatoes dataset.

### Objective of this Project
The objective is to explore the dataset and build several models with different complexities.

### Dataset
The dataset is sourced from this [Kaggle Competition](https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/overview).

#### Train Data
- **PhraseId:** Identification integer of one phrase. Several PhraseIds may be related to one same SentenceId.
- **SentenceId:** Identification of one sentence.
- **Phrase:** String, the actual text to be exploited by the model, but it needs to be preprocessed.
- **Sentiment:** Ratings range from 0 (negative) to 4 (positive).

#### Test Data
- **PhraseId**
- **SentenceId**
- **Phrase**

### Data Preprocessing

In this stage (first model, binary data supervised learning), two preprocessing steps have been performed:
1. Converting the Sentiment column (scaled from 0 to 4) to a binary target (negative 0, positive 1).
2. Cleaning the Phrase: removing whitespaces, numbers, punctuations, lowercasing all characters, tokenizing, and lemmatizing it.

### Roadmap
- [ ] Unbalanced dataset -> explore possibilities to balance it.
- [ ] Machine Learning supervised with binary target -> use the train dataset as it is labeled and split into train/test for this model.
  - [X] First version done
  - [ ] Finetuning this ML supervised.
- [ ] Another model: ML unsupervised or DL?
