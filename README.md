# Credit_Risk_Analysis
Supervised Machine Learning and Credit Risk

## Overview of the analysis: Explain the purpose of this analysis.
Created 6 different statistical models to help predict loan risk for a credit card company. I ran tests using a variety of data, such as applicant's annual income, credit limit, home ownership and more. After testing each model and running predictions, I then ran accuracy scores and classification reports for each model to assess how well it predicted. I used Python to create and run my models. 


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
  * Results Summary: Very low precision score, 

__4. Combination (Over and Under) Sampling__<br>
![](https://github.com/scaslo2/Credit_Risk_Analysis/blob/main/Analysis%20Photos/combination.png)
  * Balanced accuracy score: 0.62907 (how often the classifier predicts correctly)
  * Results Summary: Veyr low precision score but a good sensitivity score. This is represented in the accaracy score. 

__5. Balanced Random Forest Classifier__<br>
![](https://github.com/scaslo2/Credit_Risk_Analysis/blob/main/Analysis%20Photos/random_forest.png)
  * Balanced accuracy score: 0.99895 (how often the classifier predicts correctly)
  * Results Summary: Perfect sensitivty score, strong precision score. Near perfect accuracy score. This is a great model to use!

__6. Easy Ensemble Classifier__<br>
![](https://github.com/scaslo2/Credit_Risk_Analysis/blob/main/Analysis%20Photos/ensemble.png)
  * Balanced accuracy score: 0.99895 (how often the classifier predicts correctly)
  * Results Summary: Perfect precision and sensitivity scores and a near perfect accuracy score. This is a great model to use!
<br>


## Summary: 
__Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.__





