# Drug Review Condition Prediction
This project leverages the Drug Review Dataset (2018) to predict a patient's condition based on their review of a drug. The project implements a Multinomial Naive Bayes (MNB) model using TF-IDF Vectorization for feature extraction.

## Project Overview
The dataset contains patient reviews of drugs, their ratings, conditions, and other metadata. This project aims to:
- Predict the condition a drug is used for based on patient reviews.
- Evaluate the accuracy and effectiveness of the MNB classifier for text-based classification tasks.

## Dataset
The dataset used for this project is publicly available on Kaggle (UCI ML Drug Review dataset)

## Dataset Features
- uniqueID: Unique identifier for the review.
- drugName: Name of the drug.
- condition: The condition the drug was used for.
- review: Patient's review of the drug.
- rating: Patient's rating of the drug on a 10-star scale.
- date: Date of the review.
- usefulCount: Count of how many people found the review useful.
  
## Modeling Approach
- Data Preprocessing:Removed rows with missing values in review or condition.
- Label-encoded the target variable (condition).

- Feature Engineering:Used TF-IDF Vectorization to convert text data into numerical features.
Included unigrams and bigrams, with a maximum of 5000 features.

- Model Training: Trained a Multinomial Naive Bayes model on the processed training data.
- Evaluation: Measured performance using accuracy and generated a classification report.

## Results
The model achieved an accuracy of 52.11% on the test dataset, demonstrating its potential to classify conditions based on patient reviews.

## Project Workflow
 - Exploratory Data Analysis (EDA):
Visualized the distribution of ratings and analyzed text data.

- Preprocessing:Handled missing values.
Applied TF-IDF vectorization.
- Model Building:Trained the MNB classifier.
Predicted and evaluated the results on the test dataset.

##  Future Work
- Experiment with advanced models like XGBoost or Transformer-based architectures (e.g., BERT).
- Explore techniques like sentiment analysis to enhance feature extraction.


