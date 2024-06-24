# Amazon Product Rating Prediction

![NINTCHDBPICT000636804302](https://github.com/JaiBhatia19/London-Bike-Rides-Dashboard/assets/143343337/e7f5f805-f1dc-4a9d-aab3-964f9365f67c)

## Project Overview
Using natural language processing (NLP) and machine learning to predict Amazon product ratings from customer reviews. This project leverages the Amazon musical products review data.

## Tools and Technologies
- Python
- NLP
- Machine Learning

## Data
The dataset used for this project is sourced from:
- [Amazon Musical Instruments Reviews](https://cseweb.ucsd.edu/~jmcauley/datasets/amazon_v2/)

## Notebook
The data preprocessing and modeling are performed in the following Jupyter Notebook:
- [rating_prediction.ipynb](rating_prediction.ipynb)

### Data Acquisition and Preprocessing
- The Amazon Musical Instruments dataset is parsed and loaded into a pandas DataFrame.
- A sample of 20,000 reviews is taken for analysis.
- Data cleaning steps include handling missing values and selecting relevant features such as 'overall', 'verified', 'reviewText', and 'summary'.
- Additional features like 'reviewLength' and 'logLength' are derived.
- Visualizations are created to understand the distribution of ratings and review lengths.

### Feature Engineering
- Reviews are preprocessed using Spacy for tokenization and lemmatization.
- Stop words are removed to clean the text data.
- Binary feature extraction and TF-IDF feature representation are implemented to transform the text data into numerical features.

### Model Building
- A regression model is built using binary feature representation.
- The model's performance is evaluated using metrics such as R-squared and RMSE (Root Mean Squared Error).
- Another regression model is built using TF-IDF feature representation for improved performance.

### Model Evaluation
- The binary feature model achieved an R-squared of 0.457 on the training set.
- The TF-IDF model improved performance, achieving a Train RMSE of 1.193 and a Test RMSE of 1.227.

## Report
The final report can be found here:
- [final_report.pdf](final_report.pdf)

## Instructions
1. Clone the repository.
2. Open the `rating_prediction.ipynb` notebook and run all cells.

## Findings
- The TF-IDF model provided better performance compared to the binary feature model.
- Text features such as review length and whether a review was verified were significant predictors of product ratings.
