🚢 Titanic - Exploratory Data Analysis & Machine Learning

This project performs **exploratory data analysis (EDA)** and **data cleaning** on the Titanic dataset from the famous [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic). The goal is to understand the key features that influenced passenger survival and prepare the dataset for machine learning modeling.

 📌 Project Objectives

- Understand the structure and content of the Titanic dataset
- Perform data cleaning: handle missing values, drop irrelevant columns
- Perform exploratory data analysis:
  - Survival rates by sex, class, age, family size, etc.
  - Correlation between variables
- Engineer new features (e.g., Title extraction, FamilySize)
- Prepare the dataset for machine learning models


🗂️ PROJECT STRUCTURE

titanic-eda-ml/
│
├── data/ # Original dataset files from Kaggle
│ ├── train.csv
│ ├── test.csv
│ └── gender_submission.csv
│
├── notebooks/
│ └── titanic_eda.ipynb # Main notebook for EDA and preprocessing
│
├── outputs/
│ ├── cleaned_train.csv # Cleaned version of training data
│ └── plots/ # Visualizations from EDA
│
├── scripts/ # Optional Python scripts for automation
│ └── clean_data.py
│
├── requirements.txt # List of required Python packages
├── README.md # Project overview and instructions
└── .gitignore # Files/folders to ignore in version control


🧪 Dataset Description

The dataset is split into:

- `train.csv`: used to build models (includes `Survived` target)
- `test.csv`: used to predict survival (ground truth not included)
- `gender_submission.csv`: baseline submission assuming all females survived

Key variables

| Variable    | Description                           |
|-------------|---------------------------------------|
| `Survived`  | Survival (0 = No, 1 = Yes)            |
| `Pclass`    | Passenger Class (1 = 1st, 3 = 3rd)    |
| `Sex`       | Gender                                |
| `Age`       | Age in years                          |
| `SibSp`     | Siblings/Spouses aboard               |
| `Parch`     | Parents/Children aboard               |
| `Fare`      | Ticket Fare                           |
| `Embarked`  | Port of Embarkation (C/Q/S)           |

📊 Key EDA Insights

- **Sex**: Females had a much higher survival rate than males.
- **Pclass**: 1st class passengers had the highest survival rate.
- **Age**: Younger children had higher survival rates.
- **FamilySize**: Having 1–3 family members increased survival chances.
- **Title**: Titles like "Mrs", "Miss", and "Master" indicated higher survival.

🧹 Features Engineered
Title: Extracted from the Name column
FamilySize: Calculated from SibSp + Parch + 1
Converted Sex and Embarked to numeric
Handled missing values in Age, Embarked, and dropped Cabin

🛠️ TOOLS & TECHNOLOGIES USED
A combination of industry-standard tools and Python libraries was used to analyze the data, visualize trends, and prepare the dataset for predictive modeling.


| Category              | Tool/Library         | Purpose                                         |
|-----------------------|----------------------|-------------------------------------------------|
| Programming           | Python               | Core language for data analysis and scripting   |
| Data Manipulation     | Pandas               | Handling and preprocessing tabular data         |
| Numerical Computing   | NumPy                | Numerical operations and array handling         |
| Data Visualization    | Matplotlib           | Creating static plots and charts                |
|                       | Seaborn              | Advanced statistical plotting and heatmaps      |
| Notebook Environment  | Jupyter Notebook     | Interactive analysis and visual storytelling    |
| Version Control*      | Git & GitHub         | Version control and project collaboration       |

📎 Acknowledgements
Kaggle Titanic Competition
Inspired by data science learning projects


📬 Let's Connect!  
I’m always open to feedback, collaboration, or freelance data science and data analyst projects.
📫 Connect with me on [LinkedIn](https://www.linkedin.com/in/rudrappakattimani/)
