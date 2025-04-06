# 🌍 Life Expectancy Data Preprocessing

This project focuses on cleaning and preprocessing a Life Expectancy dataset for further analysis or model building. 
The dataset includes a wide range of health, economic, and demographic indicators across multiple countries and years.

---

## 📁 Dataset Overview

The dataset contains **2,938 rows** and multiple features, including:

- **Country**
- **Year**
- **Status** (Developed / Developing)
- **Life Expectancy**
- **Adult Mortality**
- **Infant Deaths**
- **Alcohol Consumption**
- **Percentage Expenditure**
- **Hepatitis B**, **Polio**, **Diphtheria** Immunizations
- **Measles Cases**
- **BMI**
- **GDP**, **Population**
- **Schooling**
- **HIV/AIDS**
- **Thinness** indicators
- **Income Composition of Resources**

---

## 🔧 Preprocessing Steps

1. **Import Libraries**  
   Imported necessary Python libraries such as `pandas`, `numpy`, `seaborn`, `matplotlib`, and `scikit-learn`.

2. **Read Dataset**  
   Loaded the dataset using `pandas.read_csv()`.

3. **Sanity Check of Data**  
   - Checked data types and column information using `.info()` and `.describe()`
   - Verified dataset shape and value ranges.

4. **Exploratory Data Analysis (EDA)**  
   - Visualized feature distributions
   - Plotted correlations
   - Checked for missing data patterns

5. **Missing Values Treatment**  
   - Handled null values using mean/median imputation
   - Used interpolation or forward/backward fill for time-related data

6. **Outliers Treatment**  
   - Detected outliers using IQR and visual tools like boxplots
   - Treated or capped extreme values

7. **Duplicates and Garbage Value Treatment**  
   - Removed duplicate rows
   - Validated value ranges and removed garbage (e.g., negative values where not possible)

8. **Normalization**  
   - Applied Min-Max Scaling or Standardization using `sklearn.preprocessing`

9. **Encoding Categorical Variables**  
   - Used one-hot encoding for columns like `Status`

> Final dataset shape: **(2938, 213)**  
> Dtypes: `float64` (20 columns), `bool` (193 columns)

---

## 📊 Output

- Cleaned and preprocessed dataset ready for modeling or visualization
- Feature-engineered version with encoded categorical values and normalized features

---


