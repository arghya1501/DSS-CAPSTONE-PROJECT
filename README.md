# 📊 Customer Churn Analysis Project

A comprehensive data analytics capstone project by **Arghyadip Pandey**, integrating Python, Power BI, Excel, and PowerPoint to explore customer churn behaviors and build actionable business insights.

---

## 📁 Project Files

```
Churn_Analysis/
├── Churn_Analysis.ipynb         # Jupyter Notebook for data cleaning, EDA, and modeling
├── Churn_Analysis.pbix          # Power BI report with interactive churn dashboards
├── Churn_Analysis.xlsx          # Excel sheet for data preprocessing and preparation
└── Churn_Analysis.pptx          # Project presentation summarizing insights and findings
```

---

## 🎯 Project Objective

To identify and analyze key drivers of customer churn through data integration and visualization techniques, and to provide strategic recommendations for customer retention using real business data.

---

## 🛠️ Tools & Technologies

- **Python (Jupyter Notebook)** for data cleaning and EDA  
- **Microsoft Excel** for initial data preparation  
- **Power BI** for dashboarding and visualization  
- **PowerPoint** for presenting insights  

---

## 📥 Data Collection

- **Data Sources:** Provided by a telecom company, including:
  - Customer Data
  - Churn History
  - Internet Usage
  - Telecom Churn Data Dictionary
- **File Formats:**
  - `.txt`, `.csv` for data
  - `.xlsx`, `.pbix`, `.ipynb` for analysis

---

## 🧹 Data Preparation Highlights

### 🔹 In Excel:
- Loaded text files using **Get Data > From Text/CSV**
- Handled missing/null values and duplicates
- Standardized formats (e.g., `DOB`, `SeniorCitizen`, `TotalCharges`)
- Ensured categorical consistency (`Yes` vs `yes`, etc.)

### 🔹 In Python:
```python
# Checking and handling missing values
df.isnull().sum()

# Filling missing numerical values
df['TotalCharges'] = df['TotalCharges'].astype(float)
df['TotalCharges'].fillna(df['TotalCharges'].mean(), inplace=True)

# Handling categorical data
df['Churn'] = df['Churn'].map({'Yes': 1, 'No': 0})
df['Contract'] = df['Contract'].astype('category')

# Removing duplicates
df.drop_duplicates(inplace=True)
```

---

## 📊 Exploratory Data Analysis (Python)

- **Churn Rate:** 26.54%
- **Monthly Charges:** Higher among churned customers
- **Contract Types:** Short-term contracts associated with higher churn
- **Payment Method:** Electronic/Mailed checks show higher churn rates
- **Tenure:** Lower tenure associated with higher churn

---

## 📈 Power BI Dashboard Highlights

- Visual breakdown by **Contract Type**, **Payment Method**, and **Tenure**
- Filterable insights based on **Demographics** and **Service Usage**
- Identification of **high-churn segments**
- Interactive visuals for actionable decisions

---

## 🧠 Insights & Recommendations

- Focus on converting short-term contracts into long-term ones
- Encourage automatic payments (linked to lower churn)
- Personalize service plans for high-risk customers
- Enhance service quality and billing transparency

---

## ✅ Conclusion

A multi-platform analysis combining Python, Excel, and Power BI to deliver a strategic framework for improving customer retention. This project exemplifies the use of data-driven approaches in identifying churn drivers and implementing retention strategies.

---

## 📬 Contact

**Arghyadip Pandey**  
📧 Email: [arghyadippandey15@gmail.com](mailto:arghyadippandey15@gmail.com)

---

*This project was submitted as part of the Certification in Data Analytics (Batch: DAB15).*
