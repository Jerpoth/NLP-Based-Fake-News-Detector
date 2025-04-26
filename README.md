# Fake News Detection using NLP

## Overview

This project implements a fake news detection system using Natural Language Processing (NLP) techniques. It utilizes a dataset of news articles labeled as either "real" or "fake" to train machine learning models capable of distinguishing between the two.

## Context

Fake news is a pervasive issue with significant impacts on society. This project aims to address this problem by providing an automated tool for identifying potentially misleading news articles.

## Dataset

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

To install all the dependencies, run:

