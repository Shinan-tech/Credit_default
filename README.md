# Credit_default

## Our objectives:
### To build a logistic regression model to predict the credit default rate  

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
7. In the original dataset, we realised there are non-value in the dataset. After discussion, we have two solutions. The first one is to remove the rows with empty value, which is around 10% of the whole dataset; the second solution is use mean to fill empty cell.
8. We seperated our dataset into train(80% of the total dataset) and test(20% of the total dataset). 
9. We don't know which way could bring us a better result, therefore we ran the logistic regression twice with different solutions on the train dataset. There is no much difference on the regression table results.
10. We used the test data to calculate the correctly predction rate.



## Our conclusion:
1. Increasing of the loan_income ratio statistically significant increased the default risk.
2. Category G statistically significant increased the default risk comparing to Category A.
3. The model predicted >80% correctly.
