# Accelerating Medicines Partnership Parkinson's Disease (AMP-PD) Progression Prediction
**Analysis of Protein and Peptide Levels Over Time to Predict Progression of 
Parkinson’s Disease**
#### Team Members: [Ruixin Lou](https://github.com/RuixinLou), [Emmanuel Ruhamyankaka](https://github.com/ruhamyakmc), [Sukhpreet Sahota](https://github.com/5ukhy21), [Jiaxin Ying](https://github.com/helenyjx)

## Project Video
https://www.youtube.com/watch?v=QoQLmDszVCw

## Kaggle Link
https://www.kaggle.com/competitions/amp-parkinsons-disease-progression-prediction

## Project Description
Parkinson's Disease is a neurodegenerative disorder that affects millions of people worldwide. The progression of the disease is commonly measured using the Movement Disorder Society - Unified Parkinson's Disease Rating Scale (MDS-UPDRS) scores, which assess motor and non-motor symptoms. The Accelerating Medicines Partnership Parkinson's Disease (AMP-PD) Progression Prediction Kaggle competition seeks to discover unforeseen patterns and predict the progression of Parkinson's Disease using clinical UPDRS scores and peptide and protein abundance data captured from cerebrospinal fluid (CSF) samples. Unlike previous studies that have solely focused on statistical models and peptide/protein levels, our project and this data science competition will be unique in approach as it combines this information with clinical data and analyzes it all together, potentially contributing to a better understanding of the disease and ultimately leading to improved treatments for patients through UPDRS scores.

This study provides a detailed walkthrough of crucial assumptions made, the development of the predictive models, and the limitations for predicting UPDRS scores to determine Parkinson's Disease progression using peptide and protein abundance data from CSF samples. Analysis and findings from this data science competition can potentially lead to the development and breakthroughs of new medicines and medical techniques, such as specific pharmacotherapies, that aim to slow the progression or cure Parkinson's Disease.

## Data
This project consisted of 3 files: clinical trial data, peptide data, and protein data.
All associated training and test files are provided in the source repository `00_source_data`.
You can download all datasets here: https://www.kaggle.com/competitions/amp-parkinsons-disease-progression-prediction/data

## Project Methodology Flowchart
<p align="center">
<img width="441" alt="ML Flowchart Parkinsons Disease" src="https://user-images.githubusercontent.com/112578035/233227559-adc39a5a-e096-4091-8232-87c743a950d2.png">
</p>

## Final Predicting Results
<img width="868" alt="Screen Shot 2023-04-21 at 1 24 28 AM" src="https://user-images.githubusercontent.com/112274822/233547580-7602d5fc-60ad-4ecb-8e8a-553711f86e42.png">

<img width="266" alt="Screen Shot 2023-04-21 at 1 23 14 AM" src="https://user-images.githubusercontent.com/112274822/233547449-05f0b87f-539e-428d-9654-1d1721d91eb9.png">

## Report Summary
The report focuses on using machine learning techniques to predict the progression of Parkinson's Disease. The study involved merging three datasets, including clinical data, peptide, and protein data, into a single dataframe. The data was pre-processed using a MinMaxScaler to scale the numerical features within a range of 1s and 0s, which is more appropriate for this case than StandardScaler since it does not assume a normal distribution of the data. Using the MinMaxScalar ensured that all features were based on a similar scale and prevented any one feature from exerting a disproportionate influence on the others (p. 11). Once the features were scaled, the team used a 10-fold split to evaluate the performance of the models, in which the models were trained on 9 portions of the data and then tested on the remaining portion. This method was repeated 10 times with different evaluations before being averaged to obtain a more reliable estimate of each model’s performance (p. 11). The study identified the best machine learning model for this problem, which was the ensemble stacking model. The model achieved the lowest SMAPE of 57.2, which is essential for clinical decision-making and patient care. The report highlights the complexity of using machine learning techniques to predict the progression of Parkinson's Disease and recommends that machine learning tools be considered complementary to current medical procedures. The report also identifies several limitations and areas for future work, including seeking insights from medical professionals, resolving missing values with imputation, and partnering with foundations and organizations dedicated to finding a cure for Parkinson's Disease. Overall, the report's significance lies in its contribution to the understanding of Parkinson's Disease and the potential use of machine learning techniques to predict its progression.

## How-To-Get-Started Guide
Open your terminal and run the following lines in order: 

1. `git clone git@github.com:5ukhy21/IDS-705_ML-Project_Parkinson-Disease-Analysis.git`

2. `cd 10_code`

From here you'll be able to run any of notebooks in the repository without any trouble (with the exception of changing directory of source data).

The notebook used to generated the results found from our report is `best score.ipynb`

## Data Dictionary
<img width="677" alt="image" src="https://user-images.githubusercontent.com/112578035/233228025-017d0611-df3f-461b-a0a5-aa0ee7b044b5.png">
