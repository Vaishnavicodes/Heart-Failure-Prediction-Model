# Heart-Failure-Prediction-Model
Prediction model to detect heart failure in patients. Dataset from Kaggle 

The dataset used for this code, is from kaggle 
    **https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction?resource=download**


-----------------------------------------------------------------------------------------------------------
**Context**
Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 31% of all deaths worldwide. Four out of 5 CVD deaths are due to heart attacks and strokes, and one-third of these deaths occur prematurely in people under 70 years of age. Heart failure is a common event caused by CVDs and this dataset contains 11 features that can be used to predict a possible heart disease.

**Goal**
This notebook aims to predict whether a patient is prone to heart disease or not according to a set of features.

**Dataset Specifications**
The dataset contains multiple numerical and categorical features. Therefore, it is necessary to propose a method to handle categorical features. One-Hot-Encoding or Label-Encoding (mapping categorical features to integers) might be useful for this purpose.
This dataset also contains some missing values. Although using `df.describe()` might not reveal this problem since missing values are specified with `0` rather than `NaN`, by taking a look at the records of this dataset can help a lot to find missing values.

**Dataset Attributes**
1) Age: Age of the patient [years]
2) Sex: Sex of the patient [M: Male, F: Female]
3) ChestPainType: Chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
4) RestingBP: Resting blood pressure [mm Hg]
5) Cholesterol: Serum cholesterol [mg/dl] (includes missing values)
6) FastingBS: Fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
7) RestingECG: Resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
8) MaxHR: Maximum heart rate achieved [Numeric value between 60 and 202]
9) ExerciseAngina: Exercise-induced angina [Y: Yes, N: No] "Exercise-induced angina" refers to a condition where a person experiences chest pain or discomfort during physical activity or exercise. Angina is typically caused by reduced blood flow to the heart muscles due to narrowed or blocked coronary arteries. During exercise, the heart requires more oxygen and blood flow to meet the increased demand, and if the arteries are narrowed, the heart may not receive enough oxygen-rich blood, leading to angina symptoms.
10) Oldpeak: Oldpeak = ST [Numeric value measured in depression]
11) ST_Slope: The slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping] "ST_Slope" refers to the slope of the peak exercise ST segment, which is a part of the electrocardiogram (ECG) waveform. The ST segment represents the interval between the end of the S wave (ventricular depolarization) and the beginning of the T wave (ventricular repolarization) on the ECG.
12) HeartDisease: Output class [1: heart disease, 0: Normal]
