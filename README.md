# student-dropout-prediction
Machine Learning project to predict student dropout using demographic and academic features. Built with Python, scikit-learn, and Random Forest classifier (ROC-AUC ~0.94).
## Project Overview

**Goal**: Build a predictive model to help universities identify at-risk students early and implement retention strategies.  
**Task**: Binary classification (Dropout = 1 / Graduate or Enrolled = 0).  
**Dataset**: [Predict students' dropout and academic success](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success) from UCI Machine Learning Repository (4,424 samples, 37 features).

**Key steps**:
- Data collection and exploration
- Data cleaning and feature engineering
- Exploratory Data Analysis (EDA)
- Model development: Logistic Regression (baseline) and Random Forest (advanced)
- Model evaluation (Accuracy, Precision, Recall, F1-score, ROC-AUC)
- Feature importance analysis
- Conclusions and recommendations for improvement

## Repository Structure
student-dropout-prediction/

├── MLB_StudentDropoutPrediction.ipynb      
├── cleaned_student_dropout.csv           
├── data.csv                              
└──README.md            


## How to Run the Project

### Option 1: Google Colab (Recommended)

1. Open https://colab.research.google.com
2. Go to **File → Upload notebook** and upload `Student_Dropout_Prediction.ipynb`
3. Download the dataset ZIP:  
   https://archive.ics.uci.edu/static/public/697/predict+students+dropout+and+academic+success.zip
4. Unzip it and upload the `data.csv` file to your Colab session (click the folder icon on the left → Upload)
5. Run all cells sequentially (Runtime → Run all)

### Option 2: Run Locally

# 1. Clone the repository

git clone https://github.com/alalyyy/student-dropout-prediction.git
cd student-dropout-prediction

# 2. (Optional) Create a virtual environment

python -m venv venv
source venv/bin/activate        # Linux/Mac
venv\Scripts\activate           # Windows

# 3. Install dependencies

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# 4. Download and place data.csv in the project folder
# 5. Start Jupyter Notebook
jupyter notebook

## Open Student_Dropout_Prediction.ipynb and run the cells.
##  Requirements
The project uses standard Python libraries. Install them with:

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Results Summary

Baseline Model (Logistic Regression): ROC-AUC ≈ 0.85
Advanced Model (Random Forest): ROC-AUC ≈ 0.94, Accuracy ≈ 0.91
Key predictors: Success rate in the 1st semester, tuition fee status, age at enrollment

# License
The original dataset is licensed under CC BY 4.0.
This project code is provided for educational purposes.
Acknowledgments

Dataset authors: Valentim Realinho et al.
UCI Machine Learning Repository

Feel free to fork and contribute!
