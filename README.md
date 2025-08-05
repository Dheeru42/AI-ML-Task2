
# 🧪 Exploratory Data Analysis (EDA) on Titanic Dataset

## 📁 Dataset
- **Source:** Kaggle Titanic Dataset (`Titanic-Dataset.csv`)
- **Imported Using:** `pandas`

## 🛠️ Key Steps Performed

### 1. **Import Libraries**
- Core libraries: `pandas`, `matplotlib`, `seaborn`
- For handling warnings: `warnings`

### 2. **Load the Dataset**
```python
df = pd.read_csv("Titanic-Dataset.csv")
```

### 3. **Basic Data Exploration**
- **Shape of dataset:** Number of rows and columns
- **Preview of data:** `df.head()`
- **Column descriptions:** Manual comment block explaining each feature like `Survived`, `Pclass`, `Sex`, `Age`, etc.

### 4. **Data Types & Missing Values**
- Used `df.info()` to check data types
- Used `df.isnull().sum()` to identify missing values
- Used `df.describe()` for statistical summary
- Used `df.duplicated().sum()` to check for duplicates

### 5. **Clean & Save the Dataset**
- Saved cleaned data to a new CSV: `new_df.csv`
- Reloaded data and dropped the index column `Unnamed: 0`

### 6. **Target Variable Exploration**
- Count of survivors (`Survived`)
- Bar Chart and Pie Chart for `Survived` column

### 7. **Univariate Analysis**
- **Categorical Columns:** Bar plots and pie charts for `Pclass`, `Sex`, `Embarked`, etc.
- **Continuous Columns:** Histograms for `Age`, `Fare`

### 8. **Bivariate Analysis**
- Bar plots comparing `Survived` with:
  - `Sex`
  - `Pclass`
  - `Embarked`
  - `SibSp`, `Parch`

### 9. **Box Plots for Outlier Detection**
- Plotted boxplots for numerical columns:
  - `Age`
  - `Fare`

### 10. **Correlation Analysis**
- Generated correlation matrix using `.corr()`
- Visualized using `sns.heatmap()`

---

## 📊 Visualizations Used
- Bar Charts
- Pie Charts
- Histograms
- Box Plots
- Heatmap

---

## 📝 Conclusion
This EDA provided insights into survival distribution, class and gender impact, missing value handling, and correlations. It set a strong foundation for further feature engineering and model building.
