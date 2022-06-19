# Credit_Risk_Analysis

## Table of Contents
- [Overview of Project](#OverviewProject)
- [Results](#Results)
  * [Resolving Class Imbalance Models](#RCI)
    - [Random Oversampling](#RO)
    - [SMOTE Oversampling](#SMOTE)
    - [Undersampling](#US)
    - [Combiation of Oversampling and Undersampling](#COMB)
  * [Classifier](#RFC)
    - [Balanced Random Forest](#BRF)
    - [Balanced Random Forest Scaled](#BRFS)
    - [Easy Ensemble](#EE)
    - [Easy Ensemble Scaled](#EES)

- [Summary](#Summary)
- [Resources](#Resources)

## <a name="OverviewProject"></a>Overview of Project

We will be creating different models to evaluate credit risk from a group of data [[3]](#3). Given that applicants that are risky are significantly less than safe loans, we will be using different models with unbalanced classes. We will oversample, undersample, use a combination of both [[1]](#1) in addition to using other models such as random forests and ensemble learning [[2]](#2). We will evaluate which model or models give us more accurate results.

## <a name="Results"></a>Results


### <a name="RCI"></a>Resolving Class Imbalances Models

In this subsection we will be evaluating the differences between oversampling, using SMOTE for oversampling, undersampling and using a combination of them [[1]](#1). Out data consists of 68,470 low-risk applicants and 347 high-risk applicants.  Given this, we will be mainly evaluating the model's performance with predicting high-risk applications.  

#### <a name="RO"></a>Random Oversampling

  * **Counter** - Low risk 51,366 applicants & high risk 51,366 applicants.
  * **Balanced Accuracy Score** - 65.74%.
  * **Confusion Matrix** -  72 accurately predicted high risk, 29 inaccurately preducted high risk
  * **Classification Report** -  1%  high risk prescicion, 71% recall, 2% f1 score.  

In the random oversampling the model picked data from the already excisting high risk applicant data, and created extra entries of it. We ended up with 51,366 low-risk applicants and 51,366 high risk applicants. 
In this case a small percentage of the values predicted to be high risk are actually high risk. Yet of the samples that were actually high risk 71% were accurately predicted to be so. 

<p align="center"> <img src="Resources/RandomOverSampler/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 1: Random Oversampling Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/RandomOverSampler/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 2: Random Oversampling Confusion Matrix</p> 

<p align="center"> <img src="Resources/RandomOverSampler/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 3: Random Oversampling Classification Report Imbalanced</p> 


#### <a name="SMOTE"></a>SMOTE Oversampling

  * **Counter** - Low risk 51,366 applicants & high risk 51,366 applicants.
  * **Balanced Accuracy Score** - 66.22%.
  * **Confusion Matrix** -  64 accurately predicted high risk, 37 inaccurately preducted high risk
  * **Classification Report** -  1%  high risk prescicion, 63% recall, 2% f1 score.  

<p align="center"> <img src="Resources/SmoteOversampling/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 4: SMOTE Oversampling Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/SmoteOversampling/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 5: SMOTE Oversampling Confusion Matrix</p> 

<p align="center"> <img src="Resources/SmoteOversampling/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 6: SMOTE Oversampling Classification Report Imbalanced</p> 


#### <a name="US"></a>Undersampling

  * **Counter** - Low risk 246 applicants & high risk 246 applicants.
  * **Balanced Accuracy Score** - 54.42%.
  * **Confusion Matrix** -  70 accurately predicted high risk, 31 inaccurately preducted high risk
  * **Classification Report** -  1%  high risk prescicion, 69% recall, 2% f1 score.  

<p align="center"> <img src="Resources/Undersampling/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 7: Undersampling Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/Undersampling/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 8: Undersampling Confusion Matrix</p> 

<p align="center"> <img src="Resources/Undersampling/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 9: Unersampling Classification Report Imbalanced</p> 

#### <a name="COMB"></a>Combination of Oversampling and Undersampling

  * **Counter** - Low risk 68,430 applicants & high risk 68,460 applicants.
  * **Balanced Accuracy Score** - 64.47%.
  * **Confusion Matrix** -  73 accurately predicted high risk, 28 inaccurately preducted high risk
  * **Classification Report** -  1%  high risk prescicion, 72% recall, 2% f1 score.  

<p align="center"> <img src="Resources/CombinationSampling/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 10: Combination Sampling Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/CombinationSampling/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 11: Combination Sampling Confusion Matrix</p> 

<p align="center"> <img src="Resources/CombinationSampling/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 12: Combination Sampling Classification Report Imbalanced</p> 

### <a name="RFC"></a>Classifier Models

In this subsection we will be evaluating boostrapping and Random Forest [[2]](#2). Out data consists of 68,470 low-risk applicants and 347 high-risk applicants.  Given this, we will be mainly evaluating the model's performance with predicting high-risk applications.  


#### <a name="BRF"></a>Balanced Random Forest

  * **Balanced Accuracy Score** - 78.85%.
  * **Confusion Matrix** -  71 accurately predicted high risk, 30 inaccurately preducted high risk
  * **Classification Report** -  3%  high risk prescicion, 70% recall, 6% f1 score.  

<p align="center"> <img src="Resources/BalancedRandomForest/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 13: Balanced Random Forest Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/BalancedRandomForest/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 14: Balanced Random Forest Confusion Matrix</p> 

<p align="center"> <img src="Resources/BalancedRandomForest/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 15: Balanced Random Forest Classification Report Imbalanced</p> 

<p align="center"> <img src="Resources/BalancedRandomForest/FeatureImportances.png" width ="70%" alt="FeatureImportances"> </p>
<p align="center"> Figure 16: Balanced Random Forest Feature Importances</p> 

#### <a name="BRFS"></a>Balanced Random Forest Scaled

  * **Balanced Accuracy Score** - 78.85%.
  * **Confusion Matrix** -  71 accurately predicted high risk, 30 inaccurately preducted high risk
  * **Classification Report** -  3%  high risk prescicion, 70% recall, 6% f1 score.  

<p align="center"> <img src="Resources/BalancedRandomForestScaled/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 17: Balanced Random Forest Scaled Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/BalancedRandomForestScaled/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 18: Balanced Random Forest Scaled Confusion Matrix</p> 

<p align="center"> <img src="Resources/BalancedRandomForestScaled/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 19: Balanced Random Forest Scaled Classification Report Imbalanced</p> 

<p align="center"> <img src="Resources/BalancedRandomForestScaled/FeatureImportances.png" width ="70%" alt="FeatureImportances"> </p>
<p align="center"> Figure 20: Balanced Random Forest Scaled Feature Importances</p> 



#### <a name="EE"></a>Easy Ensemble


<p align="center"> <img src="Resources/EasyEnsemble/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 21: Easy Ensemble Accuracy Score</p> 

<p align="center"> <img src="Resources/EasyEnsemble/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 22: Easy Ensemble Confusion Matrix</p> 

<p align="center"> <img src="Resources/EasyEnsemble/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 23: Easy Ensemble Classification Report Imbalanced</p> 

#### <a name="EES"></a>Easy Ensemble Scaled

<p align="center"> <img src="Resources/EasyEnsembleScaled/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 24: Easy Ensemble Scaled Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/EasyEnsembleScaled/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 25: Easy Ensemble Scaled Confusion Matrix</p> 

<p align="center"> <img src="Resources/EasyEnsembleScaled/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 26: Easy Ensemble Scaled Classification Report Imbalanced</p> 

## <a name="Summary"></a> Summary

In this case, we prefer models with higher recall percentages for the high-risk population than having good prescicion. It is better to incorrectly label low risk participants as high risk, and have further evaluation for them than to innacurately approve credit for people that are high risk with their credit.

From the models addressing the class imbalances we see that the combination sampling has the best high risk recall with 72%, yet compared to the other models it does not perform as well with the low risk recall having labeled 28 entries as false low risk cases. The random oversampling in this case has 71% of high risk recall (29 false low risk cases), yet the number of false high risk cases is 600 less than the one for the combination sampling. It would take additional resources to make the false risk cases be cleared as low risk. So in this case from the class imbalance models, the random oversampling is the most accurate. 

In the classifier models, we ran the models with scaled data as well as with the original data to understand their performance differences and biases. We found that the classifier models perform better with the original data sets. The balanced random forest performed particularly poorly with the scaled data, not predicting any data point as low risk. Although we would usually run the random forest with scaled data, we would have to do further documentation digging as to why the balanced forest works best with original data sets. 

Overall the classifier models perform better than the ones addressing the sample size. Of those, the Easy Ensemble AdaBoost Classifier performs the best predicting the high risk cases. 

## <a name="Resources"></a>Resources

<a name="1">[1]</a> [Loan Credit Risk Resampling Code](https://github.com/tamiespinosa/Credit_Risk_Analysis/blob/11852332e1ce9a54f127814a186441e0cd2dcf5c/credit_risk_resampling.ipynb)

<a name="2">[2]</a> [Loan Credit Risk Ensemble Code](https://github.com/tamiespinosa/Credit_Risk_Analysis/blob/11852332e1ce9a54f127814a186441e0cd2dcf5c/credit_risk_ensemble.ipynb)

<a name="3">[3]</a> [Loan Data](https://github.com/tamiespinosa/Credit_Risk_Analysis/blob/11852332e1ce9a54f127814a186441e0cd2dcf5c/Resources/LoanStats_2019Q1.csv)

[4] https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
