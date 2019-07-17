# Freedom From Uncertainity

This repository contains source codes, to all of the attempts made by me in the competition.


| File Name | Description | Creates output | LB score | Rank/Total Participants(at the time of submission) | Submission Date |
| --------- | ----------- | -------------- | -------- | ------------------------------- | ------- |
| [Baseline](https://github.com/Japkeerat/Freedom-From-Uncertainity/blob/master/Baseline.ipynb) | During exploratory data analysis it was found that a feature with attribute 'Real Lower Band' has an extremely high correlation(~1) with the target variable. So this baseline is all about using just this 1 feature and mapping it to stock price using Linear Regression algorithm. | Yes | 87.80745 | 32/351 | 17 July, 2019 |
| [Baseline-3-Models](https://github.com/Japkeerat/Freedom-From-Uncertainity/blob/master/Baseline_3_models.ipynb) | Wanted to see if it is better to build 3 different Linear Regression models based on the Company name as still the correlation was almost 1. A tweak of baseline model. Wasted a submission as validation score was less in this file and still went onto making a submission. | Yes | 87.80429 | 32/364 | 17 July, 2019 |


LB Score = max(0, (100 - Mean Absolute Eror))

50% private testing data.
