# Credit_default

## Our objectives:

### Building a logistic regression model to predict the credit default rate  

## Used linked (source):

[Our repository](https://github.com/Shinan-tech/Credit_default)

[Dataset](https://www.kaggle.com/laotse/credit-risk-dataset)

## Our work done:

1. We set up our repository on git hub named "Credit_default"
2. We found the dataset from kaggle
3. We interpreted each column in the dataset
4. We checked each variables to see if there is any outliers. If so, we removed them for further analysis
5. We visualised some independent variables and also the default / non default distribution per different categorical variables
6. We identified: person_age and cb_person_cred_hist_length are highly correlated loan_amount and and loan_percent_income are highly correlated. Therefore we removed person age as well as loan_amount.
7. In the original dataset, we realised there are NULL-values in the dataset. After discussion, we came up with two solutions to deal with the issue. The first one is to remove the rows with empty value, which is around 10% of the whole dataset; the second solution is to fill empty cells with MEAN of corresponding variables.
8. We seperated our dataset into train(80% of the total dataset) and test(10% of the total dataset). 
9. We used the test data to calculate the correctly predction rate.



## Our conclusion:

### Interpretating regression variables

Positive siginifcant Impact on default:
- loan_int_rate
- loan_percent_income
- MORTGAGE, OTHER, RENT in comparison to home_ownership OWN
- DEBTCONSOLIDATION, EDUCATION, HOMEIMPROVEMENT, MEDICAL, PERSONAL in comparison to loan_intent VENTURE
- B, C, D, E, F, G in comparison to loan_grade A

Positive siginifcant Impact on default:
- person_income
- person_emp_length

Non-significant impact on default:
- cb_person_cred_hist_length
- Y in comparison to N in default history

Interesting findings:
- There does not seem to be a difference in impact on default between loan_grade D-F
- EDUCATION followed by PERSONAL, MEDICAL seem to increase impact on default much less than DEBTCONSOLIDATION and HOMEIMPROVEMENT in comparison to loan_intent VENTURE
- MORTGAGE, OTHER, RENT seem to increase impact on default a lot in comparison to home_ownership OWN

3. We are able to predcit 86% of our data correctly with the model used
