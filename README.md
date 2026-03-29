# News Article Classification Using NLP and Machine Learning

# Overview

This project focuses on automatically classifying news articles into predefined categories such as sports, politics, business, and entertainment. It uses Natural Language Processing (NLP) and machine learning techniques to process text data and build accurate multi-class classification models.

# Objectives
Classify news articles into multiple categories
Perform text preprocessing and cleaning
Extract meaningful features using TF-IDF
Train and compare multiple machine learning models
Evaluate model performance using appropriate metrics
Dataset Description
Total records: 50,000 news articles
# Features:
Headline (text)
Category (label)
## Number of classes: 10
 1.Wellness
 2.Politics
 3.Entertainment
 4.Travel
 5.Style & Beauty
 6.Parenting
 7.Food & Drink
 8.World News
 9.Business
 10.Sports
Balanced dataset with 5,000 samples per class
# Methodology
## Data Preprocessing
 Converted text to lowercase
 Removed URLs, punctuation, and special characters
 Removed extra spaces
 Prepared clean text for modeling
# Exploratory Data Analysis
 Verified class distribution (balanced dataset)
 Visualized category distribution using bar charts
 Checked dataset quality and consistency
# Feature Engineering
 Applied TF-IDF vectorization
 Used unigrams and bigrams
 Limited features to top 5000 terms
 Converted text into numerical feature matrix

# Model Development

## Trained multiple machine learning models:
 Multinomial Naive Bayes (baseline)
 Logistic Regression (multinomial)
 Support Vector Machine (LinearSVC)

## Used:

Stratified train-test split (80/20)
Cross-validation (Stratified K-Fold)
Hyperparameter tuning using GridSearchCV

## Model Evaluation
 Accuracy
 F1-score (macro)
 Classification report
 Confusion matrix
# Results
 Multinomial Naive Bayes: ~71% accuracy
 Logistic Regression: ~73% accuracy
 LinearSVC: ~74% accuracy (best model)
 LinearSVC achieved the highest performance with balanced classification across all categories
 
# Key Features
 Multi-class text classification
 End-to-end NLP pipeline
 TF-IDF feature engineering
 Model comparison and tuning
 Interpretability using top feature words per class

# Insights
Linear models perform well on sparse TF-IDF features
Certain keywords strongly influence category prediction
Balanced dataset improves model reliability
Headlines alone can provide strong classification signals

# Technologies Used
 Python
 Pandas
 NumPy
 Scikit-learn
 Matplotlib
 
# Visualizations
 Category distribution plots
 Model comparison charts
 Confusion matrix
 Top keywords per category
 
# Future Enhancements
  Use full article text instead of headlines
  Apply deep learning models such as BERT
  Improve feature representation using embeddings
  Deploy as a web-based classification tool

# Conclusion

This project demonstrates how NLP and machine learning techniques can effectively classify news articles into multiple categories. It highlights the importance of preprocessing, feature extraction, and model selection in solving real-world text classification problems.
