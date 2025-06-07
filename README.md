# **Titanic Survival Analysis Project**
A comprehensive data analysis project exploring the Titanic dataset, featuring:
- **Complete EDA** with visualizations
- **Predictive modeling** (Logistic Regression & Random Forest)
- **Interactive dashboard** with Plotly Dash

## **📂 Project Structure**

```
titanic-analysis/
├── data/
│   └── titanic.csv            # Raw dataset
├── notebooks/
│   └── Titanic_EDA.ipynb      # Jupyter notebook with full analysis
├── scripts/
│   ├── eda.py                 # EDA script
│   ├── modeling.py            # Modeling script
│   └── app.py                 # Dash application
└── README.md                  # This file
```

## **🚀 Quick Start**

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/titanic-analysis.git
   cd titanic-analysis
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the analysis**
   - For EDA:
     ```bash
     python scripts/eda.py
     ```
   - For modeling:
     ```bash
     python scripts/modeling.py
     ```
   - For the dashboard:
     ```bash
     python scripts/app.py
     ```
     Then visit `http://127.0.0.1:8050` in your browser

## **🔍 Project Highlights**

### **1. Exploratory Data Analysis**
- Missing value treatment
- Feature engineering (Title extraction, Family size)
- Comprehensive visualizations:
  - Survival rates by class/gender
  - Age and fare distributions
  - Correlation analysis

![EDA Visualization](images/survival_by_class.png)

### **2. Predictive Modeling**
- **Logistic Regression** (78-80% accuracy)
- **Random Forest** (82-85% accuracy)
- Feature importance analysis

```python
# Model training example
rf_pipeline = Pipeline(steps=[
    ('preprocessor', preprocessor),
    ('classifier', RandomForestClassifier())
])
rf_pipeline.fit(X_train, y_train)
```

### **3. Interactive Dashboard**
- Dynamic visualizations
- Model performance comparison
- Interactive filters

## **📊 Key Findings**
1. **Women had 74% survival rate** vs 19% for men
2. **1st class passengers** survived at 63% rate vs 24% for 3rd class
3. **Children (<10 years)** had higher survival rates
4. **Family size** impacted survival chances
5. **Random Forest outperformed** Logistic Regression

## **🛠️ Dependencies**
- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- plotly
- dash

## **📧 Contact**
For questions or suggestions, please contact:
- Email-ID - adisartape19149@gmail.com
