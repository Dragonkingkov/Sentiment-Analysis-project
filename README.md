
# Sentiment Analysis
## Project Overview
A comprehensive sentiment analysis project that uses both traditional Machine Learning models and VADER (Valence Aware Dictionary and sEntiment Reasoner) to analyze tweet sentiments. The project implements multiple classification algorithms and compares their performance in identifying positive and negative sentiments.

## Dataset
Tweet data with binary sentiment labels:

- 0: Negative sentiment
- 1: Positive sentiment
Each record contains:

- ItemID: Unique identifier for each tweet
- Sentiment: Binary sentiment label
- SentimentText: The actual tweet content
## Structure
### 1. preprocessing_Training.ipynb
This notebook handles the data preparation and model training pipeline:

- Text preprocessing and cleaning
  - URL removal
  - Username (@mentions) removal
  - Hashtag cleaning
  - HTML tag removal
  - Stopword removal
  - Punctuation handling
- Feature extraction using Count Vectorization
- Model training and evaluation
- Saving trained models using joblib

### 2. Sentiment_Analysis_MLmodel_VADER.ipynb
This notebook provides the sentiment analysis implementation:

- Loading pre-trained models
- Interactive text input for analysis
- Parallel analysis using:

  - Machine Learning models
  - VADER sentiment analyzer


- Comprehensive sentiment scoring and visualization

##  Machine Learning Models Implemented

### Logistic Regression

Basic classification model
Baseline for performance comparison


### Random Forest Classifier

Ensemble learning method
Uses multiple decision trees


### AdaBoost Classifier

Boosting algorithm
Uses 100 estimators


### Ensemble Voting Classifier

Combines multiple models:

Logistic Regression
Random Forest
Support Vector Machine (SVM)


Uses 10-fold cross-validation



### VADER Sentiment Analysis

Uses VADER's sentiment intensity analyzer
Provides compound scores and normalized results
Handles:

- Emoji interpretation
- Punctuation emphasis
- Word modifiers

##  Evaluation Metrics

- Confusion Matrix for classification accuracy
- Detailed classification reports
- Model-wise accuracy comparisons
- Cross-validation results

