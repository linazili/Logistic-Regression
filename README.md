# Logistic Regression
My task was to create a logistic regression model and to predict whether the patient has 10-year risk of future coronary heart disease (CHD). The dataset includes over 4,000 records and 15 attributes.

Steps:
1. Data cleaning: replaced the missing values with the median values, as all of the attributes were treated as important.
2. Dataset split into Training set and Test set (80/20).
3. Counted coefficients, using XLMiner and was looking for Multicolinearity.
4. Created 7 models using Gretl. the right model was selected looking into significant p values and Chi Square values.
5. The selected model was perfomed on a training set. Calculated logit, Odds, Probability of CHD and Prediction.
6. Created Confusion Matrix. Used Solver to find the intercepts. Was looking for the best Recall rate, as it was more important to find more true positives rather than False Negatives.
The threshold was lowered until as many True Positives were found as posible. The cutoff of 0.1 was chosen at a sensitivity (recall) level 82%.
   
![image](https://github.com/linazili/Logistic-Regression/assets/117217908/87ba23b5-b549-43c4-9c57-58e8cc37b6b7)


Cutoff ranges are confirming that when choosing accuracy and specificity, we are sacrifying sensitivity.

![image](https://github.com/linazili/Logistic-Regression/assets/117217908/5d6f3be5-8808-4339-aecd-535cb17c7f57)


7. Counted ROC and AUC. AUC value is 70%, meaning that model has moderate discriminatory power. It is able to separate individuals who are likely to develop coronary heart disease from those who are not to some extent, but the accuracy is not extremely high.
   
![image](https://github.com/linazili/Logistic-Regression/assets/117217908/8df91f12-3427-44a1-9acc-40bf78ba75ff)


8. Model was run with the Test set and got AUC 71.66 %, recall 86%.
9. Being male, getting older and other attributes such like: cigsPerDay, prevalentStroke, sysBP and glucose statistically significantly increase the odds of getting CHD in the next 10 years.
10. Counted the prediction for any randon person of getting CHD.
    
 ![image](https://github.com/linazili/Logistic-Regression/assets/117217908/f6370f64-0d4f-4b03-a5c7-3eb3ea725154)

   
