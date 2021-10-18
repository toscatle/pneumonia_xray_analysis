# X-Ray Images Analysis for Pneumonia in Pediatric Patients
Author: Tosca Le

<!-- <img src="images/vaccine stock photo.jpeg"> -->


## Overview

This project explores a dataset of x-ray images from pediatric patients with/without pneumonia. Pneumonia is a very common inflammatory condition that is found in the lungs, primarily in the air sacs when filled with fluid or pus. Symptoms can include cough, fever, chills, and difficulty breathing. Pneumonia can be life-threatening, but particularly to infants, children and people over the age of 65 (Mayo Clinic).

The images in the dataset were selected from cohorts of patients from one to five years old from Guangzhou Women and Children's Medical Center. The data was provided by Kermany et al. on Mendeley through Kaggle datasets. All the chest x-ray images were screened for quality control, and then the diagnoses of the images were graded by two expert physicians before cleared for training.

***

## Business Problem

The Children's Medical Center has asked for assistance in partially automating the diagnosis of pneumonia in their pediatric patients. Rather than finding the best possible accuracy on a model, a deep neural network that has been clearly iterated on can help our understanding of how these models and automation work in order to help doctors confidently and efficiently diagnosis pneumonia. Broadly speaking, this can also help our understanding of AI learning and its implementation in other parts of the medical field.

***

## Data

The data was organized into three folders: train, test, and val. Each folder contains sub-folders labeled as two categories, normal and pneumonia. Within the train set there are 5216 images between the two classes, 624 in test and only 16 images in val. Since the val set contained very few images, to better balance the validation set, I randomly selected images from the test folder and moved them to the respective class within val.

***


## Methods

This project analyzes and compares neural network models based on whether or not the patient has pneumonia or not. After preparing and preprocessing the data, the dataset is split into train, test, and validataion subsets for model validation. Accuracy was used as the evaluation metric.

***


## Results

<!-- The intial baseline shows the seasonal flu vaccine target having fairly balanced classes, roughly half of respondents received the flu vaccine. 

![graph1](./images/baseline.png)

After iterating through logistic regression and decision tree models, the two models had similar ROC-AUC scores and ROC curves. 

![graph2](./images/rocauc.png)

However, the tuned decision tree (last iteration) had slightly better precision than the logistic regression and did not have as many false positives.

![graph3](./images/dtmatrix.png) -->

***


## Conclusions

<!-- The tuned decision tree had minimal false positives (number of observations where the model predicted someone will get the vaccine but they ultimately didn't) and optimize on precision, which measures the proportion of positive identifications that were actually correct.

With this model, the top three weighed feature importance were: opinion_seas_vacc_effective, doctor_recc_seasonal, and opinion_seas_risk. The first feature refers to the respondent's opinion about seasonal flu vaccine effectiveness and was categorized between 1 (very low) to 5 (very high). The last feature, opinion about risk of getting sick with seasonal flu without the vaccine also had the same value range. For seasonal flu vaccine recommendation by doctor, it was a binary yes or no question. 

Explaining the effectiveness of receiving the flu vaccine and risks of not receiving it may increase the likelihood of someone who might have doubts and could benefit from a better understanding. The Public Health Institute could provide informational materials to place in medical buildings or give to medical staff to give patients. Even if they were already planning on getting the flu vaccine, having information readily available could minimize missing people who might not be deemed at risk or assumed to have received the flu vaccine. -->

***

### Next Steps

<!-- * The survey data included H1N1-specific questions. These are likely to be highly correlated with seasonal flu attitudes and outcomes, which can affect the interpretation of the models. It would be interesting to examine these relationships or data specifically collected on seasonal flu vaccine independently in more recent years.

* Since there was such a wide range of features, including the categorical features that were omitted, it might be beneficial to simplify the analysis by examining specific subsets of features.

* This data was collected through a phone survey, which probably has barriers in itself in terms of data collection and thoroughness. Finding different ways to collect this type of data could help our analysis or present different ways for this problem to be examined.

* There are many parameters that could've been tuned or other models to explore. Our understanding of these additional iterations can help the business problem as well. -->

***

## For More Information

<!-- Please review my full analysis in my [Jupyter Notebook](./flu_vaccine_analysis.ipynb) or [presentation](./flu_vaccine_analysis_presentation.pdf).

The data for this analysis was provided by [DrivenData](https://www.drivendata.org/competitions/66/flu-shot-learning/page/210/) through the courtesy of the [United States National Center for Health Statistics](https://www.cdc.gov/nchs/index.htm).  -->

For any additional questions, please contact me at **toscatle@gmail.com**.

***

## Repository Structure

<!-- ```
├── images
├── .gitignore
├── LICENSE                          
├── README.md 
├── flu_vaccine_analysis.ipynb                                  
└── flu_vaccine_analysis_presentation.pdf                               
``` -->
