# [NBME_kaggle_competition](https://www.kaggle.com/competitions/nbme-score-clinical-patient-notes/overview)

## Before you start
To run this code, you need to go to the competition page and [download data](https://www.kaggle.com/competitions/nbme-score-clinical-patient-notes/data).  

## About the competition
![nbme_data](https://user-images.githubusercontent.com/85990934/173393496-4b2390c1-6193-4be8-bf35-698078e4c79d.jpg)
On this screenshot you can see how data is looks like, but to understand our main target let's look on one sample (row) from this dataset. 

![nbme](https://user-images.githubusercontent.com/85990934/173392755-9d69221e-6d42-47bc-a06e-3e84fd01c650.jpg)
Our target is to predict the right location of each feature word (or sequence of words) in the text.  
For example I chose "heart pounding; heart racing" feature, and as we can see "palpitations", "heart is pounding", "heart is fast" are the words related to this feature. 

For my first approach I decided to use BERT model.   
Now I am working on the second approach with different types of Deberta model.

## Results
So far I have the following results with BERT model:   
**Competition result**  
![nbme_bert_result](https://user-images.githubusercontent.com/85990934/173400621-04599367-98ca-440e-b743-1be1b3724aef.jpg)  
**Test data result**  
![nbme_bert_test_result](https://user-images.githubusercontent.com/85990934/173401489-338e0eb8-b878-4fd8-86c5-05b4fbbb927d.jpg)  
Which is not so good, but work still in progress. Will see what deberta will show.

## Possible improvements
* Try pseudo labeling
* Get more training data with exact match (already implemented)
* Try blend models
* Data augmentation (questionable)
* ...

## My personal goals
With this competition I got deeper understanding how to work with: advanced NLP problems, tokenizers, different models architectures.
