# X-Ray Images Analysis for Pneumonia in Pediatric Patients
Author: Tosca Le

<!-- <img src="images/vaccine stock photo.jpeg"> -->


## Overview

<!-- This project explores the National 2009 H1N1 Flu Survey (NHFS), which was a phone survey that asked respondents if they received the H1N1 and seasonal flu vaccines, as well as additional questions about their socioeconomic, demographic background, and opinions on illness risks and vaccine effectiveness. 

The Public Health Institute would like to focus their efforts on outreach to communities that would benefit from more seasonal flu vaccine information/resources based on features identified to affect the probability of receiving the flu vaccine the most. -->
***

## Business Problem

<!-- The goal is to understand what drives the models and which features are important in the prediction of individuals who will get the seasonal flu vaccine or not. The Public Health Institute should be able to use this understanding to minimize missing people that could've benefited from vaccine outreach and see what factors might contribute the most to individuals choosing to receive the vaccine. By knowing this, the Public Health Institute can focus their efforts on specific communities and aid in providing the necessary resources to increase vaccine rates and in return, better understand vaccine effectiveness. -->
***

## Data

<!-- The NHFS data subset includes a features and labels set. The features set contains the different survey questions while the labels set contains the target variables, which are whether the respondents received the vaccines. The dataset contains 26,707 entries including 35 features, ranging from opinion and behavioral questions to socio-economic and demographic questions.For this analysis, only the seasonal flu specific features and label will be used. -->

***


## Methods

<!-- This project analyzes and compares classification models based on whether or not the respondent received the seasonal flu vaccine. After preparing and preprocessing the data, the dataset is split into train and test subsets for model validation. Precision and ROC-AUC scores were used as evaluation metrics. -->

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
