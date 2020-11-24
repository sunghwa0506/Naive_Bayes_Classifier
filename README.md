# Naive_Bayes_Classifier

 

The goal of this assignment is to learn about the Naive Bayes Classifier (NBC).   
You will post a complete assignment using Jupyter notebook in your homepage and submit to Canvas. 
For this homework, you are not allowed to use any library because NBC is very easy to implement. 
We will use text dataset about the movie review. Your goal is predicting the sentiment.  
http://ai.stanford.edu/~amaas/data/sentiment/ (Links to an external site.)

# Below is the process.
## 1. Divide the dataset as train, development and test. 
## 2. Build a vocabulary as list. 
### a.[‘the’ ‘I’ ‘happy’ … ] 
#### You may omit rare words for example if the occurrence is less than five times
### b.A reverse index as the key value might be handy
#### {“the”: 0, “I”:1, “happy”:2 , … }

## 3.Calculate the following probability
### Probability of the occurrence
#### P[“the”] = num of documents containing ‘the’ / num of all documents
### Conditional probability based on the sentiment
#### P[“the” | Positive]  = # of positive documents containing “the” / num of all positive review documents
## 4.Calculate accuracy using dev dataset 
### Conduct five fold cross validation
## 5.Do following experiments
### Compare the effect of Smoothing
### Derive Top 10 words that predicts positive and negative class
#### P[Positive| word] 
## 6.Using the test dataset
### Use the optimal hyperparameters you found in the step e, and use it to calculate the final accuracy.  
### Use five fold cross validation for final accuracy
