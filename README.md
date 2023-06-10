# Parkinsons_Disease_Prediction

This project focuses on predicting whether a patient is suffering from Parkinson's disease based on audio/voice measures. Machine learning models are used to analyze the dataset and make predictions.

## Dataset

The dataset used in this project is stored in the file `parkinsons.data`. It contains 195 rows and 24 columns. Each column represents a different attribute related to the voice measures of the patients.

### Attribute Information:

-   **name**: ASCII subject name and recording number
-   **MDVP:Fo(Hz)**: Average vocal fundamental frequency
-   **MDVP:Fhi(Hz)**: Maximum vocal fundamental frequency
-   **MDVP:Flo(Hz)**: Minimum vocal fundamental frequency
-   **MDVP:Jitter(%), MDVP:Jitter(Abs), MDVP:RAP, MDVP:PPQ, Jitter:DDP**: Several measures of variation in fundamental frequency
-   **MDVP:Shimmer, MDVP:Shimmer(dB), Shimmer:APQ3, Shimmer:APQ5, MDVP:APQ, Shimmer:DDA**: Several measures of variation in amplitude
-   **NHR**: Measure of ratio of noise to tonal components in the voice
-   **HNR**: Measure of ratio of noise to tonal components in the voice
-   **status**: Health status of the subject (1 - Parkinson's, 0 - healthy)
-   **RPDE, D2**: Two nonlinear dynamical complexity measures
-   **DFA**: Signal fractal scaling exponent
-   **spread1, spread2, PPE**: Three nonlinear measures of fundamental frequency variation

## Findings

The following findings were observed during the analysis:

-   The dataset has a high number of patients affected by Parkinson's disease.
![download](https://github.com/pras-ops/Parkinsons_Disease_Prediction/assets/56476064/42b7bb4d-25f9-4cca-b197-b3d96dc100fc)
-   Patients affected by Parkinson's disease have high values for 
1. NHR (noise to tonal components ratio)
![download](https://github.com/pras-ops/Parkinsons_Disease_Prediction/assets/56476064/bd302c5f-bbd9-45c5-aa78-e5769257e65d)
3. HNR (ratio of noise to tonal components)
![download](https://github.com/pras-ops/Parkinsons_Disease_Prediction/assets/56476064/06b9782d-2c94-4185-9082-d1c767bcba7a)
-   The nonlinear dynamical complexity measure RPDE is high in patients affected by Parkinson's disease.
![download](https://github.com/pras-ops/Parkinsons_Disease_Prediction/assets/56476064/0ef8b956-dfef-4d5e-97bb-f2cbd761bdd8)
-   Random forest model performs better compared to other models, with an accuracy of 94%.
-   Logistic regression achieved an accuracy of 84%.
-   Decision tree, Naive Bayes, K-Nearest Neighbors, and Support Vector Machine models were also applied, but random forest yielded the highest accuracy.
-   The kappa score, a measure of agreement between predicted and true values, was calculated for the random forest model.

Please refer to the code for detailed implementation and further analysis of the dataset.

## Report

The analysis of the Parkinson's disease prediction based on audio/voice measures resulted in the following key findings:

-   Parkinson's disease can be predicted with a high level of accuracy using machine learning techniques.
-   Random forest model outperformed other models, achieving an accuracy of 94% in predicting Parkinson's disease.
-   Nonlinear dynamical complexity measure RPDE, NHR, and HNR were found to be important features in distinguishing patients with Parkinson's disease.
-   The dataset used in this project had a high number of patients affected by Parkinson's disease.

These findings indicate the potential of using audio/voice measures for early detection and diagnosis of Parkinson's disease, which can aid in providing timely medical interventions and support to patients.

Please refer to the code for detailed implementation, including data preprocessing, model training, and evaluation.
