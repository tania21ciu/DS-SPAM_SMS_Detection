# SPAM SMS Detection
## Objective
The high number of SMS spamming cases causes this case to become one of unsettling cases in society. Therefore, it is necessary to have a spam filter with the concept of SMS spam detection. This project compares the performance of Support Vector Machine (SVM) and Naive Bayes algorithm to find the appropriate algorithm for SMS spam detection. 

## Framework
1. Data Retrieving => Data spam SMS is retrieved from UCI dataset repository in http://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection. The data is consist of 5 variables with 5572 rows as basis of analysis. 
2. Data Preprocessing => consists of: 
   - Filter Stopword: for filtering words that appear frequently but doesn't give the meaning to the statement
   - Stemming: for getting the basic word (word without affixes)
   - Vectorization: using TF-IDF (Term Frequency - Inverse Document Frequency)
3. Data Splitting => The pre-processed data will be split into training data for model building and testing data for model testing.
4. Data Modeling & Data Validation => This project uses Support Vector Machine (SVM) and Naive Bayes as algorithm model. Confusion matrix is used for model validation

## Result
The Support Vector Machine (SVM) is more recommended for the SPAM detection use case. The accuracy of SVM is 97%, which is 10% higher than Naive Bayes, which is only 87%.
