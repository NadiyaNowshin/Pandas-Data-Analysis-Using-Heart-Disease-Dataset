# Pandas Data Analysis Using Heart Disease Dataset

## Project Overview

This project demonstrates fundamental **data analysis and manipulation techniques using Pandas** with a Heart Disease dataset.

The analysis focuses on loading and inspecting the dataset, understanding its structure, identifying missing values, analyzing categorical variables, selecting data using `iloc`, and filtering records based on specific conditions.

The project is designed to build practical experience with **Pandas DataFrames and data exploration workflows**.

## Dataset Information

The dataset contains medical attributes related to cardiovascular health. Each row represents an individual patient, while the columns describe demographic information, clinical measurements, and heart disease-related characteristics.

### Dataset Source

The dataset is available on Kaggle:

[Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset?select=heart.csv)

Download the `heart.csv` file from the dataset page before running the notebook.

## Attribute Information

| Attribute  | Description                                             |
| ---------- | ------------------------------------------------------- |
| `age`      | Age of the patient in years                             |
| `sex`      | Gender: `1` = Male, `0` = Female                        |
| `cp`       | Chest pain type                                         |
| `trestbps` | Resting blood pressure (mm Hg)                          |
| `chol`     | Serum cholesterol level (mg/dl)                         |
| `fbs`      | Fasting blood sugar: `1` = >120 mg/dl, `0` = ≤120 mg/dl |
| `restecg`  | Resting electrocardiographic results                    |
| `thalach`  | Maximum heart rate achieved                             |
| `exang`    | Exercise-induced angina: `1` = Yes, `0` = No            |
| `oldpeak`  | ST depression induced by exercise relative to rest      |
| `slope`    | Slope of the peak exercise ST segment                   |
| `ca`       | Number of major vessels colored by fluoroscopy (0–3)    |
| `thal`     | Thalassemia status                                      |
| `target`   | Heart disease status: `1` = Disease, `0` = No disease   |

### Thalassemia Values

* `0` = Normal
* `1` = Fixed defect
* `2` = Reversible defect

## Analysis Objectives

The project covers the following Pandas operations:

* Loading datasets into Pandas
* Inspecting DataFrame structure
* Identifying missing values
* Analyzing categorical variables
* Selecting rows and columns using `iloc`
* Filtering data using conditional expressions
* Counting records that satisfy specific conditions

## Analysis

### 1. Dataset Loading and Initial Exploration

The dataset is loaded into a Pandas DataFrame and initially inspected.

The analysis includes:

* Displaying the first five rows
* Displaying the last five rows
* Checking the shape of the dataset

These operations provide an initial understanding of the dataset's size and structure.

### 2. Dataset Structure and Missing Value Analysis

Pandas functions are used to examine the structure and completeness of the dataset.

The analysis includes:

* Displaying all column names
* Examining data types and non-null counts using `.info()`
* Identifying missing values in each column

### 3. Categorical Data Analysis

The dataset is analyzed to understand the distribution of important categorical variables.

The analysis includes:

#### Heart Disease Status

Counting patients with:

* `target = 1`: Heart disease
* `target = 0`: No heart disease

#### Gender Distribution

Counting:

* `sex = 1`: Male
* `sex = 0`: Female

### 4. Data Selection Using `iloc`

The project demonstrates positional indexing using Pandas `iloc`.

The following selections are performed:

* Selecting the first 10 rows
* Extracting the columns representing `age`, `sex`, and `chol`
* Selecting rows from index 20 to 30 and columns from index 0 to 4

This section demonstrates how positional indexing can be used to access specific portions of a DataFrame.

### 5. Data Filtering Using Conditions

Conditional filtering is used to identify specific groups of patients.

The analysis includes:

#### Patients Older Than 50

Extracting all patients whose age is greater than 50 years.

#### Heart Disease and High Cholesterol

Identifying patients who:

* Have heart disease (`target = 1`)
* Have a cholesterol level greater than 240 mg/dl

#### Combined Condition Count

Calculating the number of patients who satisfy both conditions.

## Technologies Used

* **Python**
* **Pandas**
* **Google Colab**
* **Jupyter Notebook**

## Project Structure

```text
Heart-Disease-Pandas-Analysis/
│
├── Heart_Disease_Analysis.ipynb
├── heart.csv
└── README.md
```

## How to Run

### Google Colab

Open the `.ipynb` notebook in Google Colab and run the cells sequentially.

Make sure the `heart.csv` dataset is available in the expected location.

### Local Environment

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

Navigate to the project directory:

```bash
cd YOUR_REPOSITORY
```

Install Pandas:

```bash
pip install pandas
```

Then open the notebook using Jupyter Notebook or JupyterLab.

## Author

**Nadiya Nowshin**

