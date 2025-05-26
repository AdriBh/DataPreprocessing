# 🧹 Data Cleaning & Preprocessing – Titanic Dataset

## 📌 Objective
This project focuses on performing essential **data cleaning and preprocessing** tasks using the **Titanic dataset** to prepare it for machine learning models. It was completed as part of an internship assignment with the goal of learning real-world data preparation techniques.

---

## 📊 Dataset Used
The [Titanic dataset](https://www.kaggle.com/competitions/titanic/data) from Kaggle contains passenger information such as age, sex, class, and whether they survived the Titanic shipwreck.

---

## 🛠️ Tools & Libraries
- Python
- Pandas
- NumPy
- Seaborn & Matplotlib
- Scikit-learn (`LabelEncoder`, `MinMaxScaler`)

---

## 🧾 Task Breakdown

### 1. **Import & Explore the Dataset**
- Loaded the dataset using `pandas`
- Explored data types, basic statistics, and missing values using:
  - `.info()`
  - `.isnull().sum()`
  - `.describe()`

### 2. **Handle Missing Values**
- Filled missing **`Age`** values using the median.
- Filled missing **`Embarked`** values using the mode.
- Dropped the **`Cabin`** column due to 77% missing data.
  > Hypothesis: Imputing `Cabin` would be unreliable; it was better to remove it.

### 3. **Encode Categorical Features**
- Converted **`Sex`** and **`Embarked`** columns into numerical format using `LabelEncoder`.
- Printed label mappings for reference.

### 4. **Normalize Numerical Features**
- Applied `MinMaxScaler` to scale **`Age`** and **`Fare`** columns to range [0, 1].

### 5. **Outlier Detection & Removal**
- Visualized outliers using `boxplot` for `Age` and `Fare`.
- Removed outliers using the **IQR (Interquartile Range)** method.

---

## 📈 Visualizations
- Boxplots for detecting outliers in numerical features.
- (Optional: Add screenshots or saved plots if you're including them in the repo.)

---

## 📂 File Structure

├── titanic.csv # Dataset file
├── preprocessing_script.ipynb # Main Jupyter Notebook with code
├── README.md # This file


---

## ✅ Key Learnings
- Handling missing data with statistical methods.
- Label encoding for categorical variables.
- Scaling numerical data for machine learning readiness.
- Detecting and removing outliers to improve model quality.

---


## ⭐ Acknowledgements
Thanks to [Kaggle](https://www.kaggle.com/) for providing the dataset and [scikit-learn](https://scikit-learn.org/) for preprocessing tools.


