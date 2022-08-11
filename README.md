# Credit_Risk_Analysis
Supervised Machine Learning and Credit Risk

## Overview of the analysis:
Created 6 different statistical models to help predict loan risk for applicants at a credit card company. For the first three models, I oversampled the data using the RandomOverSampler and SMOT algorithms, and undersampled the data using the ClusterCentroids algorithm. Then I used a combined approach of over- and undersampling using the SMOTEEN algorithm. For my last two models I focused on reducing bias by using the BalancedRandomForestClassifier and EasyEnsembleClassifier machine learning models. 
<br>

The data set I use, measures a wide variety of variables such as applicant's annual income, credit limit, home ownership and more. After fitting and testing each model, I then ran accuracy scores and classification reports for each model to assess how well it performed and to determined which model or models are the best.


## Results: 
__Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.__

__1. Naive Random Sampling__<br>
![](https://github.com/scaslo2/Credit_Risk_Analysis/blob/main/Analysis%20Photos/naive.png)
  * Balanced accuracy score: 0.6516  (how often the classifier predicts correctly)
  * Results Summary: Precision is low for high risk, indicating a large number of false positives. More so, this indicates an unreliable positive classification. With an F1 score as low as 0.02 and an accuracy score of only 0.65, this model is not great at classifying high risk applications.
  

__2. SMOTE Oversampling__<br>
![](https://github.com/scaslo2/Credit_Risk_Analysis/blob/main/Analysis%20Photos/smote.png)
  * Balanced accuracy score: 0.64406 (how often the classifier predicts correctly)
  * Results Summary: With precision at only 0.01 for high risk, it is too low and indicates a large number of false positives. Because of this it is an unreliable positive classification. At 0.02 the F1 score is much too low and with an accuracy score of only 0.64, this model is also not great at classifying high risk applications.

__3. Undersampling__<br>
![](https://github.com/scaslo2/Credit_Risk_Analysis/blob/3e97a14ef71adb7859de2904bf46086fcdfb4122/Analysis%20Photos/undersampling.png)
  * Balanced accuracy score: 0.52274 (how often the classifier predicts correctly)
  * Results Summary: Fot our undersampling model, our accuracy and recall scores are 0.52 and 0.46 respectively, which is too low. Our precision score may look good with a total average of 0.99 but when we look further we can see that the precision score for high risk applications is a measly 0.01. From this we can conclude that this model is not a good model for us to use.

__4. Combination (Over and Under) Sampling__<br>
![](https://github.com/scaslo2/Credit_Risk_Analysis/blob/main/Analysis%20Photos/combination.png)
  * Balanced accuracy score: 0.62907 (how often the classifier predicts correctly)
  * Results Summary: Similar to the undersampling model, for our combination model we have a low recall or sensitivity score of 0.55 meaning there will be a low rate of correctly predicted high risk applicants. Our precision score is once again seemingly great overall but has a low precision when it comes to predicting high risk applicants. This is all reflected in the okay F1 score of 0.7. 

__5. Balanced Random Forest Classifier__<br>
![](https://github.com/scaslo2/Credit_Risk_Analysis/blob/main/Analysis%20Photos/random_forest.png)
  * Balanced accuracy score: 0.99895 (how often the classifier predicts correctly)
  * Results Summary: This model has a strong Precision score for predicting high risk loans and a perfect score in predicting low risk loans. To add to this, our accuracy score is strong 0.99 and our senisitivity score is a perfect 1.0! All in all, this is a strong model for us to use.

__6. Easy Ensemble Classifier__<br>
![](https://github.com/scaslo2/Credit_Risk_Analysis/blob/main/Analysis%20Photos/ensemble.png)
  * Balanced accuracy score: 0.99895 (how often the classifier predicts correctly)
  * Results Summary: Just as the balanced random forest model, this model has a perfect sensitivity score of 1.0 and a near perfect accuracy score of 0.99. But this model surpasses the random forest model in its precision score, with a perfect score of 1.0! With these scores, the easy ensemble classifier seems to be a really good model to use.
<br>


## Summary: 
__Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.__
After fitting, testing, and analyzing all of the models the two I would recommend would be the balanced random forest classifier and the easy ensemble classifier. These are the two models that are tailored to reducing biases. In both models the F1 score, recall or sensitivity score, precision score, and accuracy score were all very high, leading us to believe that they would be best at classifying accurately. Our only concern would be that maybe these models could have been overfit, however our sample size seems to be large enough to combat this. Just to be safe, it may be wise to re-run these two models and adjusting the noise and random sample size to see if we can get similar scores. 




