# Predicting-Loan-Defaulters
A Project on predicting Loan Defaulters. This will be the same approach for Credit Card Payment defaulters as well.

## Data Source:

Since the Datasets used are large, please refer to them on my Kaggle account. 
[Click Here for Datasets](https://www.kaggle.com/ajithganapathihegde/predicting-loan-defaulters)


## R Code: 

There is only one R Code file and its in Markdown Format. 
[Click Here for RCodes folder](https://github.com/ajithgh/Predicting-Loan-Defaulters/tree/main/RCodes)

Once we load the Dataset, we divide them to Categorical and Numerical to find out % of missing values. 

Then We engage in Data Enhancement using exisiting columns with relationships. We also engage in some other Data CLeaning and finally use Median Impute for imputing Numerical Values. 
PS: Imputation only works on Blank cells and not on '0's

Then we used ```dummyVars``` for Dummification of all categorical columns; cleaned column names and Balanced Train/Test datasets using ROSE Sampling method. 

We the build 4 Models:
+ ```RF``` (Accuracy: 90%+)
+ ```gbm``` (Accuracy: 70%)
+ ```Naive Bayes```
+ ```rpart```

Lastly we predicted on the test_file using gbm method, but you can try with RF by subsetting the Data with Top 50 features. 



## Conclusion: 

Using RF model is the best way to predict as you can get above 90% accuracy. Refer to the [Presentation deck](https://github.com/ajithgh/Predicting-Loan-Defaulters/blob/main/Results/Predicting%20Loan%20Defaulters%20-%20Results.pptx) for more details. 
