There is only one Code file with all the parts in it. Please note, all Data files used are in Kaggle as they are large to be uploaded here. 


Once we load the Dataset, we divide them to Categorical and Numerical to find out % of missing values. 

Then We engage in Data Enhancement using exisiting columns with relationships. We also engage in some other Data CLeaning and finally use Median Impute for imputing Numerical Values. 
PS: Imputation only works on Blank cells and not on '0's

Then we used ```dummyVars``` for Dummification of all categorical columns; cleaned column names and Balanced Train/Test datasets using ROSE Sampling method. 

We the build 4 Models:
+ RF (Accuracy: 90%+)
+ gbm (Accuracy: 70%)
+ Naive Bayes
+ rpart

Lastly we predicted on the test_file using gbm method, but you can try with RF by subsetting the Data with Top 50 features. 

