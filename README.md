# Freedom From Uncertainity

This repository contains source codes, to all of the attempts made by me in the competition.


| File Name | Description | Creates output | LB score | Rank/Total Participants(at the time of submission) | Submission Date |
| --------- | ----------- | -------------- | -------- | ------------------------------- | ------- |
| [Baseline](https://github.com/Japkeerat/Freedom-From-Uncertainity/blob/master/Baseline.ipynb) | During exploratory data analysis it was found that a feature with attribute 'Real Lower Band' has an extremely high correlation(~1) with the target variable. So this baseline is all about using just this 1 feature and mapping it to stock price using Linear Regression algorithm. | Yes | 87.80745 | 32/351 | 17 July, 2019 |
| [Baseline-3-Models](https://github.com/Japkeerat/Freedom-From-Uncertainity/blob/master/Baseline_3_models.ipynb) | Wanted to see if it is better to build 3 different Linear Regression models based on the Company name as still the correlation was almost 1. A tweak of baseline model. Wasted a submission as validation score was less in this file and still went onto making a submission. | Yes | 87.80429 | 32/364 | 17 July, 2019 |
| [Baseline-3-Models-with-KAMA](https://github.com/Japkeerat/Freedom-From-Uncertainity/blob/master/Baseline_3_models_with_KAMA.ipynb) | I issed a feature during EDA called KAMA. This feature was extremely strongly related to the Price and graphically it almost looked like there is a data leakage. Created both single and 3 model baseline for this feature and the one with better validation score was submitted. | Yes | 89.76469 | 27/369 | 17 July, 2019 |
| [All-MA-3-Models](https://github.com/Japkeerat/Freedom-From-Uncertainity/blob/master/All_MA_3_linear_model.ipynb) | Using all the Moving average features together with a mean of those and then splitting it for all three companies and built linear model for each. Validation method changed to look more like testing data. | Yes | 91.96365 | 24/377 | 18 July, 2019 |
| [All-MA-3-Models-RFE](https://github.com/Japkeerat/Freedom-From-Uncertainity/blob/master/All_MA_3_linear_model_RFE.ipynb) | Above the previous file, applied Random Feature Elimination technique to find the best combination of features among Moving Averages for each type and then build a model. Though the validation score improved, LB score on public test data decreased. According to the distribution of public and private in testing data, I highly believe this would improve on private testing data once competition is over. The plot in the NB explains why I think so. | Yes | 91.87966 | 24/383 | 18 July, 2019 |

LB Score = max(0, (100 - Mean Absolute Eror))

50% private testing data.
