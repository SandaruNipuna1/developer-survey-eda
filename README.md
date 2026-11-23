# 📊 SurveyLens: Public Survey & Opinion Data Explorer

## 📌 Overview

**SurveyLens** is a Data Science project focused on exploring, cleaning, and preparing the Stack Overflow Developer Survey 2026 dataset. Using Python's data analysis and visualization libraries, the project investigates developer demographics, employment, programming language preferences, database technologies, and other survey trends.

The project is being developed as part of the **Data Science Virtual Internship at SkillMe**, progressing through exploratory data analysis, data cleaning, and feature engineering.

## 🎯 Objectives

- Explore and understand a real-world survey dataset.
- Analyze developer demographics and employment patterns.
- Investigate programming language popularity.
- Explore database technologies currently used and preferred for the future.
- Identify missing data and assess data quality.
- Clean and standardize selected categorical data.
- Engineer useful features for further analysis.
- Apply categorical encoding techniques.
- Visualize findings using Python.

## 📂 Dataset

**Source:** Stack Overflow Developer Survey 2026

- **Rows:** 30,903
- **Columns:** 212
- **Type:** Public survey dataset
- **Format:** CSV

The dataset contains responses about developers' demographics, professional backgrounds, technologies used, and technology preferences.

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## 🔍 Analysis & Implementation

### Week 1 – Exploratory Data Analysis (EDA)

#### 1. Data Exploration
- Dataset overview using `head()`, `info()`, and `describe()`
- Examined dataset dimensions and data types

#### 2. Missing Data Analysis
- Identified missing values using `isnull().sum()`
- Examined missing-value counts and percentages

#### 3. Developer Demographics & Employment
- Analyzed employment status distributions
- Explored age distributions
- Compared employment categories

#### 4. Geographic Analysis
- Identified countries with the highest number of survey responses
- Visualized the top 10 countries

#### 5. Programming Language Analysis
- Explored programming languages developers have worked with
- Processed multi-select responses using `split()` and `explode()`
- Visualized the most frequently reported programming languages

#### 6. Database Technology Analysis
- Investigated databases currently used by developers
- Explored databases developers want to work with in the future
- Compared current usage and future interest

#### 7. Group Comparison
- Used `groupby()` to compare average work experience across employment categories

#### 8. Data Visualization
- Created visualizations using Matplotlib to communicate patterns and distributions found within the survey data.

### Week 2 – Data Cleaning & Feature Engineering

#### 1. Category Inspection
- Inspected selected categorical columns for inconsistent formatting.
- Checked leading/trailing whitespace and capitalization differences.
- Implemented a reusable `clean_categories()` function.

#### 2. Missing Value Handling
- Filled missing values in selected categorical columns with `Unknown`.
- Applied median imputation to missing `WorkExp` values.
- Created a `WorkExp_WasMissing` indicator to preserve information about originally missing values.

#### 3. Feature Engineering
- Created an `ExperienceLevel` feature using `pd.cut()`.
- Grouped respondents into three categories:
  - Junior
  - Mid
  - Senior

#### 4. Categorical Encoding
- Applied one-hot encoding using `pd.get_dummies()`.
- Encoded selected categorical features, including Employment, Education, and ExperienceLevel.

#### 5. Validation & Export
- Re-ran the Week 1 employment and work experience comparison using cleaned data.
- Compared results to verify that the original group averages were preserved.
- Exported the cleaned dataset to `data/survey_clean.csv`.
- Reloaded the exported CSV and verified its shape, columns, and selected missing-value counts.

**Note:** Inspection of the selected category columns did not reveal capitalization or whitespace variations that reduced the unique category count. This finding was documented rather than artificially changing valid survey categories.

## 📈 Key Learning Outcomes

- Working with a real-world dataset containing many columns
- Performing exploratory data analysis with Pandas
- Handling multi-select survey responses
- Identifying and analyzing missing data
- Applying appropriate missing-value strategies
- Standardizing categorical data
- Creating new features through feature engineering
- Applying one-hot encoding
- Validating data transformations
- Creating data visualizations
- Communicating data-driven findings

## ▶️ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/SandaruNipuna1/developer-survey-eda.git
   ```

2. Navigate to the project folder:

   ```bash
   cd developer-survey-eda
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib jupyter
   ```

4. Download the Stack Overflow Developer Survey 2026 dataset and place `survey_results_public.csv` in the project directory.

5. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Run the notebooks:
   - `developer_survey_eda.ipynb` – Week 1 EDA
   - `developer_survey_cleaning.ipynb` – Week 2 Data Cleaning & Feature Engineering

The Week 2 notebook generates the cleaned dataset at `data/survey_clean.csv`.

## 📁 Project Structure

```text
developer-survey-eda/
│
├── developer_survey_eda.ipynb
├── developer_survey_cleaning.ipynb
├── data/
│   └── survey_clean.csv
├── survey_results_public.csv
├── survey_results_schema.csv
└── README.md
```

**Note:** Dataset CSV files are excluded from the GitHub repository because of their size. Download the original survey dataset separately and generate the cleaned dataset by running the Week 2 notebook.

## 👨‍💻 Author

**Sandaru Nipuna**

Data Science Undergraduate | Python & Machine Learning Enthusiast

## 🎓 Internship

**Data Science Virtual Internship – SkillMe**

- Week 1: Exploratory Data Analysis
- Week 2: Data Cleaning & Feature Engineering

---

⭐ This project represents my hands-on learning journey in Data Science, from exploring real-world datasets to preparing data for further analysis and machine learning.
