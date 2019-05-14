# Machine Learning Report: Error Analysis
## Introduction to Computer Programming in Engineering and Science 360-420-DW - 00003
## Jordana Marciano

## Distributions of Model Accuracy

## Analysis of different error types

-the amount of confidence we can put in our model

Each time you run the classification model, you should be getting a different accuracy. Why? (hint: lines 148-150 in DataSet.java)
Each time we run the classification model, we should be getting a different accuracy because the Collections.shuffle(fullDataSet) is shuffling the elements in the list of data points so that they are randomly assigned new positions. Therefore, 

What is a sensible baseline against which we should compare our model's performance? (hint: line 200 in DataSet.java)
A sensible baseline against which we should compare our model's performance is 


-the types of errors that our classifier makes

What is a

False Positive?
A false positive is when you receive a test result that is positive but in reality the result is negative.

False Negative?
A false negative is when you receive a test result that is negative but in reality the result is positive.

Extend your analysis in the previous step (with the 1000 runs) to keep track of Recall and Precision as well.

What makes these two measures different?
The difference between the Recall measure and the Precision measure is that Recall is a measure of completeness or quantity where an algorithm returns most of the relevant results. However, Precision is a measure of exactness or quality where an algorithm returns more relevant results rather than irrelevant results.

What are sensible baseline for each of these measures?
A sensible baseline for each of these measures would be 1 where the closer we are to 1, the more precise and accurate we are.

How do the above results change with the hyperparameter k?
The above results change with the hyper parameter k because k is the number of closest neighbors that are used to determine the class of a data point. Therefore, the larger the k value the harder it is to find the nearest class since the computer has to search through more neighbors until it can make a label prediction. In addition, the hyperparameter k should not be an even number in order to avoid ties for the closest neighbor.
