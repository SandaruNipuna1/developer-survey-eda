# 📊 SurveyLens: Public Survey & Opinion Data Explorer

## 📌 Overview

**SurveyLens** is an exploratory data analysis (EDA) project focused on exploring the Stack Overflow Developer Survey 2026 dataset. The project uses Python's data analysis and visualization libraries to uncover patterns in developer demographics, employment, programming language preferences, and database technologies.

This project was completed as part of **Week 1 of the Data Science Virtual Internship at SkillMe**.

## 🎯 Objectives

- Explore and understand a real-world survey dataset.
- Analyze developer demographics and employment patterns.
- Investigate programming language popularity.
- Explore database technologies currently used and preferred for the future.
- Identify missing data and assess data quality.
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

## 🔍 Analysis Performed

### 1. Data Exploration
- Dataset overview using `head()`, `info()`, and `describe()`
- Examined dataset dimensions and data types

### 2. Missing Data Analysis
- Identified missing values using `isnull().sum()`
- Examined missing-value counts and percentages

### 3. Developer Demographics & Employment
- Analyzed employment status distributions
- Explored age distributions
- Compared employment categories

### 4. Geographic Analysis
- Identified countries with the highest number of survey responses
- Visualized the top 10 countries

### 5. Programming Language Analysis
- Explored programming languages developers have worked with
- Processed multi-select responses using `split()` and `explode()`
- Visualized the most frequently reported programming languages

### 6. Database Technology Analysis
- Investigated databases currently used by developers
- Explored databases developers want to work with in the future
- Compared current usage and future interest

### 7. Group Comparison
- Used `groupby()` to compare average work experience across employment categories

### 8. Data Visualization
Created visualizations using Matplotlib to communicate patterns and distributions found within the survey data.

## 📈 Key Learning Outcomes

- Working with a real-world dataset containing many columns
- Performing exploratory data analysis with Pandas
- Handling multi-select survey responses
- Identifying and analyzing missing data
- Applying grouping and aggregation techniques
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

4. Ensure the survey CSV file is placed in the project directory.

5. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

6. Open `developer_survey_eda.ipynb` and run the cells.

## 📁 Project Structure

```text
developer-survey-eda/
│
├── developer_survey_eda.ipynb
├── survey_results_public.csv
├── survey_results_schema.csv
└── README.md
```

## 👨‍💻 Author

**Sandaru Nipuna**

Data Science Undergraduate | Python & Machine Learning Enthusiast

## 🎓 Internship

Completed as part of the **Data Science Virtual Internship – Week 1** at **SkillMe**.

---

⭐ This project represents my hands-on learning journey in Data Science and Exploratory Data Analysis.
