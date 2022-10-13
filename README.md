# Credit_Risk_Analysis

## Overview of the Analysis
Credit card risk is a huge problem in the world. With good loans easily outnumbering risky loans, it is hard to pinpoint how to create an automated system to check if one should be approved or not. So, I was tasked with employing multiple techniques to train and evaluate models that deal with unbalanced classes suc as this. I was give  data from LendingClub, a peer-to-peer lending service company to research the following techniques:
* Naive Random Oversampling
* SMOTE Oversampling
* Undersampling
* Combination (Over and Under) Sampling
* Balanced Random Forest Classifier
* Easy Ensemble AdaBoost Classifier
Here are my findings!
## Results
### Naive Random Oversampling
![Naive_Random_Sampling](https://user-images.githubusercontent.com/107770394/195466531-2cfe2b0b-4b0d-46e8-94f5-3ad50b126703.png)
![NRO_BAS](https://user-images.githubusercontent.com/107770394/195466569-6ecff7bd-aeb7-4791-b957-07bc64370dea.png)
* The balanced accuracy score is 62.94%
* The precision for high risk is 1%, while low risk is 100%, with an average of 99%
* The recall score is 57% for high risk, while low risk is 57%, with an average of 66%
### SMOTE Oversampling
![Smote_Oversampling](https://user-images.githubusercontent.com/107770394/195467389-b8265389-c1a0-4749-9f88-ff5d8b7d6d7f.png)
![SO_BAS](https://user-images.githubusercontent.com/107770394/195467405-56fd341b-07cc-404a-bac2-e90467b39f64.png)
* The balanced accuracy score is 62.77%
* The precision for high risk is 1%, while low risk is 100%, with an average of 99%
* The recall score is 62% for high risk, while low risk is 63%, with an average of 63%
### Undersampling
![Undersampling](https://user-images.githubusercontent.com/107770394/195467704-5f9e2adb-1fbd-4803-91a4-065efb41ed77.png)
![under_BAS](https://user-images.githubusercontent.com/107770394/195468032-6e353bf0-2684-4a84-975e-8b2d26c0808d.png)
* The balanced accuracy score is 52.94%
* The precision for high risk is 1%, while low risk is 100%, with an average of 99%
* The recall score is 61% for high risk, while low risk is 45%, with an average of 45%
### Combination (Over and Under) Sampling
![Combination_Sampling](https://user-images.githubusercontent.com/107770394/195467941-8a6dbde9-fda3-4399-8502-5ef5a488b7bf.png)
![combo_BAS](https://user-images.githubusercontent.com/107770394/195467957-9877996e-ffb1-4fb5-8961-84e0834d7764.png)
* The balanced accuracy score is 65.48%
* The precision for high risk is 1%, while low risk is 100%, with an average of 99%
* The recall score is 70% for high risk, while low risk is 61%, with an average of 61%
### Balanced Random Forest Classifier
![Balanced_Random_Forest_Classifier](https://user-images.githubusercontent.com/107770394/195468161-08a4869d-5624-49c8-b875-d31574ce376e.png)
![BRFC_BAS](https://user-images.githubusercontent.com/107770394/195468190-7a11c0d9-f0a2-4695-9492-e61a478ce0f5.png)
* The balanced accuracy score is 78.85%
* The precision for high risk is 3%, while low risk is 100%, with an average of 99%
* The recall score is 70% for high risk, while low risk is 87%, with an average of 87%
### Easy Ensemble AdaBoost Classifier
![Easy_Ensemble_AdaBoost_Classifier](https://user-images.githubusercontent.com/107770394/195468340-54fc51c0-2121-4a48-9026-cd925fdddf28.png)
![EEAC_BAS](https://user-images.githubusercontent.com/107770394/195468369-bb769790-f04e-4cad-9b98-3c148fead6ff.png)
* The balanced accuracy score is 93.17%
* The precision for high risk is 9%, while low risk is 100%, with an average of 99%
* The recall score is 92% for high risk, while low risk is 94%, with an average of 94%
## Summary
As we can see, each model gave us differing results. Looking at just the balanced accuracy score alone, the Easy Ensemble AdaBoost was the clear winner here, with a score of 93.17%, whereas the others ranged from 52% to 78%, with the undersampling method giving us our lowest total. With precision being near identical it is hard to gauge any results from this. However, with the recall score, we see another clear winner, once again the Easy Ensamble AdaBoost Classifier, with an average score of 94%, the others ranging from 45% to 87%, with undersampling once again taking last place. With this knowledge, my recommendation would be the Easy Ensemble AdaBoost Classifier when trying to predict credit risk.
