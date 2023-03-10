# linear_regression_salary
## Overview
The goal of this project was to utilize machine learning models to analyze credit card risks. Oversampling, undersampling, and a combination of the two were done to identify the best way to properly train the model. After this, Balanced Random Forest Classifier and Easy Ensemble Classifier were both used to evaluate the performance of the created models. The goal was to identify a reliable way to minimize the threat of credit card risk for potential consumers. 

### Results of Balanced Accuracy, Precision, and Recall Scores
The scores for each model are as follows:
* RandomOverSampler:

 ![RandomOverSampler](https://user-images.githubusercontent.com/111502918/213198421-e7cae699-3128-462f-96a5-96e57a15ad7d.PNG)

* SMOTE Oversampler (Balanced Accuracy Score of 0.651) :

![SMOTE_Oversampling](https://user-images.githubusercontent.com/111502918/213198508-60a68c3b-cea3-40e9-8be5-5fca4267b154.PNG)

* ClusterCentroids Undersampling (Balanced Accuracy Score of 0.516):

![ClusterCentroids_Undersampling](https://user-images.githubusercontent.com/111502918/213198585-bb12a619-7171-4f59-be62-0c5339b5fcc4.PNG)

* SMOTEEEN Combination (Balanced Accuracy Score of 0.650): 

![SMOTEEEN_Combo](https://user-images.githubusercontent.com/111502918/213198649-01b8251d-1691-41fe-ac23-12eb6c470bb7.PNG)

* Balanced Random Forest Classifier (Balanced Accuracy Score of 0.796):

![brfc_model](https://user-images.githubusercontent.com/111502918/213200678-2680dd5a-0937-4559-92ff-e3b97d07e664.PNG)

* Easy Ensemble AdaBoost (Balanced Accuracy Score of 0.925)

![adaboost_model](https://user-images.githubusercontent.com/111502918/213200820-1a632d6f-c3d4-4414-8698-342206e56219.PNG)




#### Summary
As expected, each model comes with its own pros and cons. In this example, ClusterCentroids undersampling has the lowest balanced accuracy score along with lower F1 and recall scores accross the board. Both the SMOTE and SMOTEEEN models have similar balanced accuracy scores with the SMOTE model leading in terms of recall and F1 scores. However, due to a significantly higher balanced accuracy score and higher recall and F1 scores, my recommendation would be to utilize the Easy Ensemble AdaBoost model.
