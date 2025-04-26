# Fake News Detection using NLP

## Overview

This project implements a fake news detection system using Natural Language Processing (NLP) techniques. It utilizes a dataset of news articles labeled as either "real" or "fake" to train machine learning models capable of distinguishing between the two.

## Context

Fake news is a pervasive issue with significant impacts on society. This project aims to address this problem by providing an automated tool for identifying potentially misleading news articles.



### Description

The dataset consists of 72,134 news articles, with 35,028 labeled as real and 37,106 as fake. It is a merged dataset from four popular news datasets (Kaggle, McIntire, Reuters, BuzzFeed Political), designed to prevent overfitting and provide ample text data for training.

### Columns
-   **Serial number**: Starting from 0.
-   **Title**: Heading of the news article.
-   **Text**: Content of the news article.
-   **Label**: 0 = fake, 1 = real.

## Dependencies

-   numpy
-   pandas
-   matplotlib
-   seaborn
-   wordcloud
-   nltk
-   contractions
-   scikit-learn
-   re
-   string
-   pickle



## Project Structure

-   `Fake-News-Detection-using-NLP.ipynb`: Jupyter Notebook containing the code for data preprocessing, model training, and evaluation.
-   `README.md`: Project documentation (this file).

## Usage

1.  Clone the repository:
- https://github.com/Jerpoth/NLP-Based-Fake-News-Detector.git
3.  Open and run the `Fake-News-Detection-using-NLP.ipynb` notebook using Jupyter.

## Data Preprocessing

The data preprocessing steps include:

-   **Data Cleaning:** Removing missing values and irrelevant columns.
-   **Text Processing:**
    -   Expanding contractions.
    -   Removing special characters and punctuation.
    -   Tokenization.
    -   Removing stopwords.

## Model Training and Evaluation

The following models were trained and evaluated:

-   Logistic Regression
-   Multinomial Naive Bayes
-   Random Forest Classifier
-   Decision Tree Classifier
-   Gradient Boosting Classifier
-   AdaBoost Classifier

The best performing model was the **Random Forest Classifier**, with the following metrics:

| Model                      | Accuracy (Training) | Accuracy (Test) | Precision | Recall  | F1 Score | Training Time (secs) |
| -------------------------- | ------------------- | --------------- | --------- | ------- | -------- | -------------------- |
| Logistic Regression        | 0.9175              | 0.9150          | 0.9138    | 0.9286  | 0.9211   | 0.67                 |
| MultinomialNB              | 0.8496              | 0.8486          | 0.8542    | 0.8641  | 0.8592   | 0.02                 |
| Random Forest Classifier   | 0.9999              | 0.9378          | 0.9152    | 0.9737  | 0.9436   | 189.36               |
| Decision Tree Classifier   | 0.9999              | 0.9105          | 0.9073    | 0.9273  | 0.9172   | 25.26                |
| Gradient Boosting Classifier | 0.9265              | 0.9260          | 0.9071    | 0.9599  | 0.9327   | 199.66               |
| AdaBoost Classifier        | 0.9201              | 0.9196          | 0.9130    | 0.9391  | 0.9258   | 38.12                |

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


