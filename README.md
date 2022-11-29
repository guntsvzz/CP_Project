# EEG Chronic stress
This project aims to reproduct Akkaradet Experiment EEG Chronic stress which classify stress and non-stress
under pre-examination condition
##Objectives :
To find feature important and decent model
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
    - Extraction 32 channels to 16 channels
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

## Limitation :
 - less samples
## Future Work :
 - Collecting the same participants after post-examination
## Reference :
 - EEG Based Classification of Long-Term Stress Using Psychological Labeling
