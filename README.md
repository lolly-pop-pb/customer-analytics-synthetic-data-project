# **Synthetic Customer Dataset for Retail Store**

A complete end-to-end project for generating, analyzing, and modeling a **200,000-customer synthetic dataset** suitable for machine learning tasks such as clustering, regression, and exploratory analytics.

## Ideal For
- Data science practice  
- Machine learning workflow demonstration  
- Retail analytics modeling  
- Teaching / portfolio use  
## 📁 Project Structure

```plaintext
├── synthetic_data_generation.ipynb      
├── analysis_and_modeling.ipynb          
├── Synthetic_customer_data.csv          
├── README.md
└── REPORT- Synthetic Customer Dataset for Retail Store.docx
```

## Key Features
### 1. Synthetic Dataset Generation
-	Gender, Age Group, Income Level
-	Shopping Frequency
-	Product Type (randomized by age & income)
-	Salary based on income brackets
-	Monthly purchases based on shopping habits
### 2. Statistical Scaling
- Small sample of 10 customers → scaled to 200,000 via frequency distribution.
### 3. Noise & Realism
-	Random salary ranges
-	Purchase variability
-	Product-type randomness
-	Diverse customer behavior patterns
### 4. Exploratory Data Analysis
-	Distributions (Age, Income, Product Type…)
-	Correlation matrix
-	Scatter plots
-	Cluster visualization
### 5. Machine Learning
#### Clustering (K-Means)
-	Used on salary, purchase count, shopping frequency
-	Segments high-spenders, rare shoppers, etc.
#### Regression (Linear Regression)
-	Predicts monthly purchase counts
-	Achieved **R² ≈ 0.88**
#### Classification (Random Forest)
-	Attempt to classify Product_Type
-	Low accuracy due to highly random target variable
-	Included for learning purposes

## Key Learnings
-	Synthetic data scaling through frequency distributions
-	Feature engineering for retail datasets
-	Importance of structured vs. noisy target variables
-	Effect of feature scaling in clustering
-	Model evaluation using MSE, R², Confusion Matrix
-	Feature importance interpretation

## How to Run

### 1. Clone the Repository
```
git clone https://github.com/lolly-pop-pb/customer-analytics-synthetic-data-project.git
cd synthetic-customer-data-generator
```

### 2. Create a Virtual Environment
Creating a virtual environment isolates your project dependencies and keeps your system clean.

#### Windows
```bash
python -m venv venv
venv\Scripts\activate
```
#### Mac / Linux
```bash
python3 -m venv venv
source venv/bin/activate
```
You should now see (venv) in your terminal.

### 3. Install Dependencies
Install all required Python packages:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```
This will open the notebook interface in your browser.

### 5. Run the Notebooks in Order

#### Step 1 — Generate Synthetic Data
Open `synthetic_data_generation.ipynb` and run all cells.  
This will create: `Synthetic_customer_data.csv` (200,000 rows)

#### Step 2 — Analyze & Model the Data
Open `analysis_and_modeling.ipynb`.  
This notebook performs:
- Visualizations
- Correlation analysis
- K-Means clustering
- Regression modeling
- Random Forest classification
- Cluster interpretation

### 6. Deactivate the Virtual Environment (optional)
```bash
deactivate
```
