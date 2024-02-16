# Sentiment-Analysis-on-Movie-Reviews
Classify the sentiment of sentences from the Rotten Tomatoes dataset

## Objective of this project
My objective is to play with the dataset and build several models with different complexity. 

## Dataset
Dataset is coming from this [Kaggle Competition](https://www.kaggle.com/competitions/sentiment-analysis-on-movie-reviews/overview)
Train data is composed of : 
- PhraseId -> Identification int of one phrase. There are several PhraseId related to one same SentenceId.
- SentenceId -> Identification of one sentence.
- Phrase -> str, actual text to be exploited by the model, but it needs to be preprocessed.
- Sentiment -> Ratings goes from 0 (negative) to 4 (positive). 

## Data Preprocessing

At this stage (first model, binary data supervised learning), two preprocessing has been performed :
1 Converting Sentiment column (scale from 0 to 4) to a binary target (negative 0, positive 1).
2 Cleaning Phrase : removing whitespaces, numbers, punctuations, lower case all characters, tokenize and lemmatize it.  

## Roadmap
- [ ] Unbalanced dataset -> explore the possibilities to balance it.
- [ ] Machine Learning supervised with binary target -> use train dataset as it is labelled and split into train/test for this model.
  - [X] First version done
  - [ ] Finetuning this ML supervised
- [ ] Another model : ML unsupervised or DL ? 
