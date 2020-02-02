# Home-Credit-Default-Risk
![](https://camo.githubusercontent.com/47d477f194c6e3d03fa43e5f79179fed116ec304/68747470733a2f2f7777772e746872656574687269667479677579732e636f6d2f77702d636f6e74656e742f75706c6f6164732f323031332f30352f64656661756c742e6a7067)

Binary classification to identify potential loan defaulters in Home Credit's customer base.

## Table of contents
- [Business Problem](https://github.com/anshikaahuja/Home-Credit-Default-Risk/blob/master/README.md#business-problem)
- [Data Used](https://github.com/anshikaahuja/Home-Credit-Default-Risk/blob/master/README.md#data-used)
- [Approach](https://github.com/anshikaahuja/Home-Credit-Default-Risk/blob/master/README.md#approach)

## Business Problem
Home credit is an international non-bank financial institution, which focuses on lending to people with little or no credit history. In the US, the unbanked/underbanked population comes up to 22% households. This population is often exploited and taken advantage of by untrustworthy lenders. This project aims to aid Home Credit to predict the repayment capabilities of underbanked customers in the US, thereby providing a positive loan experience for the lender as well as the loanee.<br />

**Why is it important?**
- People with non existent or insufficient struggle to get loans
- Banks are unable to provide loans to unbanked population as it is difficult to predict their clients' repayment abilities
- This approach can be used by Home Credit and as well as other banks who strive to broaden financial inclusion
- Banks can use alternative data including telco and transactional information and machine learning models to make these predictions
- This will make sure that clients capable of repayment are not rejected and that loans are given with a principal, maturity, and repayment calendar that will empower their clients to be successful


## Data Used
The dataset used in this analysis can be found [here](https://www.kaggle.com/c/home-credit-default-risk/data). The EDA for base table, EDA for secondary tables and imputation strategies taken for base table are uploaded in the repository. <br />
[2019-12-02 Team SparQL.pptx](https://github.com/anshikaahuja/Home-Credit-Default-Risk/blob/master/2019-12-02%20Team%20SparQL.pptx)
has our final presentation.

## Approach
The data is present across various tables, each representing a factor which Home Credit uses to understand the customer behavior. The biggest challenge was to **identify the key feautures** which are important to predict whether a customer will default or not. As the first step, we performed **Exploratory Data Analysis** and tried to form a hypothesis based on intuition as well as the results from EDA. The next challenge was to fill in the missing values for which we applied **Data Imputation** strategies. We also performed **Feature Engineering** to filter out the redundant/insignificant predictors and create new ones to tailor to our needs. We used **LightGBM** to model the target variable and used **Area Under the ROC curve** as the evaluation metric. The complete code and model comparisons are available in the repository.
