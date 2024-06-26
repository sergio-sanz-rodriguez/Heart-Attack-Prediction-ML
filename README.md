# Machine-Learning Project - Ensemble Learning Architectures for Heart Disease Prediction

---

## Objective
The goal of this project is to investigate the potential of ensemble architectures to improve prediction in binary classification problems. We will utilize a heart disease database in order to detect, using machine-learning models, the presence of heart disease in patients.
   
The evaluated models include: **Logistic Regression**, **Support Vector Machine (SVM)**, **Random Forest**, **Soft-Voting**, and **Stacking**. The last three correspond to ensemble architectures.

## Data Overview

| Column | Additional Information |
|--------|------------------------|
| age | The age of the patient. |
| sex | The gender of the patient (0 = female, 1 = male). |
| cp| Chest pain type (1 = typical angina, 2 = atypical angina, 3 = non-anginal pain, 4 = asymptomatic). |
| trestbps| Resting blood pressure (in mm Hg). |
| chol | Serum cholesterol level (in mg/dl). |
| fbs | Fasting blood sugar (> 120 mg/dl) (1 = true, 0 = false). |
| restecg | Resting electrocardiographic results (0 = normal, 1 = having ST-T wave abnormality, 2 = probable or definite left ventricular hypertrophy). |
| thalach | Maximum heart rate achieved. |
| exang | Exercise-induced angina (1 = yes, 0 = no). |
| oldpeak | ST depression induced by exercise relative to rest. |
| slope | Slope of the peak exercise ST segment (1 = upsloping, 2 = flat, 3 = downsloping) |
| caa | Number of major vessels colored by fluoroscopy. |
| thall | Thalassemia (a type of blood disorder) results (3 = normal, 6 = fixed defect, 7 = reversible defect). |
| output |  0 = little risk of heart attack, 1 = high risk of heart attack |

More information about this dataset can be found here: https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset

---

## Set up your Environment



### **`macOS`** type the following commands : 



- For installing the virtual environment and the required package you can either follow the commands:

    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/bin/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```
Or ....
-  use the [Makefile](Makefile) and run `make setup` or install it manually with the following commands:

     ```BASH
    make setup
    ```
    After that active your environment by following commands:
    ```BASH
    source .venv/bin/activate
    ```

### **`WindowsOS`** type the following commands :

- Install the virtual environment and the required packages by following commands.

   For `PowerShell` CLI :

    ```PowerShell
    pyenv local 3.11.3
    python -m venv .venv
    .venv\Scripts\Activate.ps1
    pip install --upgrade pip
    pip install -r requirements.txt
    ```

    For `Git-bash` CLI :
  
    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/Scripts/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```

    **`Note:`**
    If you encounter an error when trying to run `pip install --upgrade pip`, try using the following command:
    ```Bash
    python.exe -m pip install --upgrade pip
    ```