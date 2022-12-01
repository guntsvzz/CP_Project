# EEG Chronic stress
This project aims to reproduct Akkaradet Experiment EEG Chronic stress which classify stress and non-stress under pre-examination condition
## Objectives :
- To classify chronic stress (stressed and non-stressed) based on EEG and compare it with Perceived Stress Scale (PSS) score test. 
- To explore feature importance to identify which frequency channels are highly significant in classifying chronic stress.

## Hypothesis : 
- Chronic Stress can be classified based on EEG data
- Some of the frequency band are more significant in Chronic Stress classification.

## Assumptions :
- High PSS scores can indicate chronic stress.
- EEG data doesn’t vary with personal information such as age, gender, etc.


## Member :
```
st123012	Todsavad Tangtortan
st123459	Anjana Tissera
st122053	Wanchanok Sunthorn
st123010	Tonson Praphabkul
st122876	Aiman Lameesa
```

## Dependencies :
- mne library 

## Components :
- 01 ETL
    - select 16-channels out of 32-channels
    - notch filter power line
    - filter
- 02 EDA
    - Feature Extraction (Alpha Beta Gamma) 
        - Power spectral density (PSD)
        - Asymmetry
- 03 ML Model
    - SVM
    - NB
    - KNN
    - LR
- 04 DL Model
    - CNN1D
    - LSTM

## Result :
- Out of the ML models we trained, Support Vector Machine has higher test accuracy.
- Generally, When Relative Gamma frequency band is included as a feature, Model testing accuracy is high.
- Deep Learning Models didn’t result with good accuracy.
- Accuracy of testing Akkaradet’s dataset
    - Low accuracy compared to our test dataset

## Conclusion :
- Hypothesis 1:  Some of the frequency band are more significant
    - The results show that Relative Gamma has a higher significance in classifying chronic stress
- Hypothesis 2 : Chronic Stress can be classified based on EEG data
    - Model accuracy varies with the dataset
    - Our experiment doesn't completely support this hypothesis.


## Limitation :
 - Bias Stress
 - No Consultant
 - Small Dataset

## Future Work :
 - Recording Post Examination
    - Collecting the same participants after post-examination

## Reference :
- Saeed, S. M. U., Anwar, S. M., Khalid, H., Majid, M., & Bagci, U. (2020). EEG based classification of long-term stress using psychological labeling. Sensors, 20(7), 1886.

- Minguillon, J., Lopez-Gordo, M. A., & Pelayo, F. (2016). Stress assessment by prefrontal relative gamma. Frontiers in computational neuroscience, 10, 101.

- Zhang, Y., Wang, Q., Chin, Z. Y., & Ang, K. K. (2020, July). Investigating different stress-relief methods using Electroencephalogram (EEG). In 2020 42nd Annual International Conference of the IEEE Engineering in Medicine & Biology Society (EMBC) (pp. 2999-3002). IEEE.

