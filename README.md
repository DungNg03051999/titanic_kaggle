# Titanic Kaggle Competition Project (Ranking Kaggle 233)
This project is part of the [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic/overview) competition on Kaggle. The goal is to predict the survival of passengers on the Titanic using machine learning models. This repository contains the necessary files and instructions to reproduce the analysis and models.

## Link Folder
All the works are stored in [Final_Project](https://drive.google.com/drive/folders/1013llj_6mRGDwIucsi6vYKfrb8B2hIWp?usp=sharing)


## Data
The data is given and saved in 'titanic.zip' in folder `dataset`
There are 3 CSV files after unzipping the file:
- 'train.csv'
- 'test.csv'
- 'gender_submission.csv'

Ignore the 'gender_submission.csv' because it is just the sample file to demonstrate the submission format.


## Library Installation
### Recommendation
Recommending to use Google Colab to run the notebook since it is already included all necessary libraries

### Prerequisites If Not Using Google Colab
To run the notebook, you need to have the following installed:

Python packages:
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

Jupyter Notebook 


## Notebook Description
- The notebook `Capstone.ipynb` is executed using Google Colab.
- Change the path inside the notebook corresponding to your local directory so that the code can run appropriately


# Steps To Run The Notebook
## Step 1: Connect to Google Drive
To connect to your google drive, run the first cell in the notebook:
```
from google.colab import drive
drive.mount('/content/drive')
```

## Step 2: Change the directory to 'dataset' folder
Find the first cell in Section 2 of the notebook: Loading data

Change the directory as the format followed:
```
with zipfile.ZipFile('your_path_to_titanic_zip_file', 'r') as zip_ref:
    zip_ref.extractall('original_dataset')
```

## Step 3: Change the submission directory to your chosen directory
- In Section 5.3: Logistic Regression, find the path in `base_lg_path` and `tuning_lg_path` variables
- In Section 6.1: Decision Tree, find the path in `tuning_dt_path` variable
- In Section 6.4 Random Forest, find the path in `rf_path` variable

Change all the path to your selected directory you want to save the submission.csv file for each model
```
path = 'your_path_you_want_to_save_model_prediction_result/name_model_submission.csv'
```

## Step 4: Run all the notebook
- Run all the notebook after adjusting correct directory
- The submission file will be saved in the directory you specified in `Step 3`

## Step 5: Result Submission
### My submission files are stored in the `submission` folder. There are 2 sub-folders in this folder:
- Base: saving 2 CSV files for base model prediction: Base Logistic Regression and Hyperparameter-Tuning Logistic Regression
- Tuning: saving 2 CSV files corresponding to tuning models: Decision Tree and Random Forest


### You can find the model submission after the code finished in the path from `Step 3`. Use those CSV files to submit the result on Kaggle 


# License
This program is created by [Nguyen Tri Dung](https://github.com/DungNg03051999)
