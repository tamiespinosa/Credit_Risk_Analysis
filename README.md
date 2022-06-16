# Credit_Risk_Analysis

## Table of Contents
- [Overview of Project](#OverviewProject)
- [Results](#Results)
  * [Resolving Class Imbalance Models](#RCI)
    - [Random Oversampling](#RO)
    - [SMOTE Oversampling](#SMOTE)
    - [Undersampling](#US)
    - [Combiation of Oversampling and Undersampling](#COMB)
  * [Random Forest and Bootstrapping Models](#RFC)
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


#### <a name="RO"></a>Random Oversampling

<p align="center"> <img src="Resources/RandomOverSampler/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 1: Random Oversampling Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/RandomOverSampler/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 2: Random Oversampling Confusion Matrix</p> 

<p align="center"> <img src="Resources/RandomOverSampler/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 3: Random Oversampling Classification Report Imbalanced</p> 


#### <a name="SMOTE"></a>SMOTE Oversampling

<p align="center"> <img src="Resources/SmoteOversampling/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 4: SMOTE Oversampling Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/SmoteOversampling/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 5: SMOTE Oversampling Confusion Matrix</p> 

<p align="center"> <img src="Resources/SmoteOversampling/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 6: SMOTE Oversampling Classification Report Imbalanced</p> 


#### <a name="US"></a>Undersampling

<p align="center"> <img src="Resources/Undersampling/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 7: Undersampling Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/Undersampling/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 8: Undersampling Confusion Matrix</p> 

<p align="center"> <img src="Resources/Undersampling/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 9: Unersampling Classification Report Imbalanced</p> 

#### <a name="COMB"></a>Combination of Oversampling and Undersampling

<p align="center"> <img src="Resources/CombinationSampling/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 10: Combination Sampling Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/CombinationSampling/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 11: Combination Sampling Confusion Matrix</p> 

<p align="center"> <img src="Resources/CombinationSampling/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 12: Combination Sampling Classification Report Imbalanced</p> 

### <a name="RFC"></a>Random Forest and Bootstrapping Models

#### <a name="BRF"></a>Balanced Random Forest

<p align="center"> <img src="Resources/BalancedRandomForest/BalancedAccuracyScore.png" width ="30%" alt="BalancedAccuracyScore"> </p>
<p align="center"> Figure 13: Balanced Random Forest Balanced Accuracy Score</p> 

<p align="center"> <img src="Resources/BalancedRandomForest/ConfusionMatrix.png" width ="50%" alt="ConfusionMatrix"> </p>
<p align="center"> Figure 14: Balanced Random Forest Confusion Matrix</p> 

<p align="center"> <img src="Resources/BalancedRandomForest/ClassificationReportImbalanced.png" width ="70%" alt="ClassificationReportImbalanced"> </p>
<p align="center"> Figure 15: Balanced Random Forest Classification Report Imbalanced</p> 

<p align="center"> <img src="Resources/BalancedRandomForest/FeatureImportances.png" width ="70%" alt="FeatureImportances"> </p>
<p align="center"> Figure 16: Balanced Random Forest Feature Importances</p> 

#### <a name="BRFS"></a>Balanced Random Forest Scaled

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



## <a name="Resources"></a>Resources

<a name="1">[1]</a> [Loan Credit Risk Resampling Code](https://github.com/tamiespinosa/Credit_Risk_Analysis/blob/11852332e1ce9a54f127814a186441e0cd2dcf5c/credit_risk_resampling.ipynb)

<a name="2">[2]</a> [Loan Credit Risk Ensemble Code](https://github.com/tamiespinosa/Credit_Risk_Analysis/blob/11852332e1ce9a54f127814a186441e0cd2dcf5c/credit_risk_ensemble.ipynb)

<a name="3">[3]</a> [Loan Data](https://github.com/tamiespinosa/Credit_Risk_Analysis/blob/11852332e1ce9a54f127814a186441e0cd2dcf5c/Resources/LoanStats_2019Q1.csv)

[4] https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
