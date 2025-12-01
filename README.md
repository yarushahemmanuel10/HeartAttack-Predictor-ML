# HeartAttack-Predictor-ML

## Project Overview
This project aims to predict the occurrence of heart attacks using patient health data. The dataset contains demographic, clinical, and diagnostic measurements. Using machine learning models, we can classify whether a patient is likely to experience a heart attack.

The project demonstrates the entire ML workflow: data exploration, cleaning, preprocessing, model training, evaluation, and parameter fine-tuning.

---

## Dataset
The dataset consists of 302 patient records and 14 features:

| Feature      | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| age         | Age of the patient                                                          |
| sex         | Sex of the patient                                                          |
| cp          | Chest pain type (0: Typical Angina, 1: Atypical Angina, 2: Non-anginal, 3: Asymptomatic) |
| trtbps      | Resting blood pressure (mm Hg)                                             |
| chol        | Cholesterol (mg/dl)                                                        |
| fbs         | Fasting blood sugar > 120 mg/dl (1: True, 0: False)                        |
| restecg     | Resting ECG results (0: normal, 1: ST-T wave abnormality, 2: LV hypertrophy)|
| thalachh    | Maximum heart rate achieved                                                |
| oldpeak     | Previous ST depression peak                                                |
| slp         | Slope of peak exercise ST segment                                          |
| caa         | Number of major vessels (0–3)                                             |
| thall       | Thalium stress test result (0–3)                                           |
| exng        | Exercise induced angina (1: Yes, 0: No)                                    |
| output      | Target variable (0: No heart attack, 1: Had heart attack)                  |

---

## Key Steps
1. **Data Cleaning & Exploration**
   - Checked for missing values and duplicates.
   - Analyzed distributions and correlations.
2. **Feature Preprocessing**
   - Scaled numerical features for K-NN.
   - One-hot encoded categorical variables.
3. **Model Training & Evaluation**
   - Models used: Gaussian Naive Bayes, Bernoulli Naive Bayes, Random Forest, K-Nearest Neighbors, XGBoost.
   - Evaluated using 10-fold cross-validation and F1 score.
4. **Parameter Fine-Tuning**
   - Applied GridSearchCV to optimize key parameters for each model.
5. **Final Observations**
   - Random Forest and Gaussian Naive Bayes are the best-performing models.
   - Fine-tuning improves performance and reduces variance.

---

## Installation & Usage
1. Clone the repository:  
```bash
git clone https://github.com/YOUR_USERNAME/HeartAttack-Predictor-ML.git
