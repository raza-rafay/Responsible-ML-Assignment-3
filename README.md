# Assignment 3 – Disparate Impact Audit of the COMPAS Model
Name: Rafay Raza  
GWID: G40856805

## Purpose of the Analysis
The purpose of this analysis is to conduct a disparate impact audit of a logistic regression risk model trained on the COMPAS two-year recidivism dataset. The audit evaluates whether the model produces fair outcomes across racial and sex groups by computing standard fairness metrics including Adverse Impact Ratio (AIR), Marginal Effect (ME), and Standardised Mean Difference (SMD) using the solas-ai library. Error-rate disparities (FPR and FNR) are tested for statistical significance using two-proportion z-tests. An intersectional subgroup analysis (race × sex) is also conducted, and findings are summarised in a compliance memo addressed to a hypothetical regulatory authority.

## Python Libraries Used
The following Python libraries were used in this assignment:
* pandas
* numpy
* matplotlib
* seaborn
* statsmodels
* scikit-learn
* solas-ai
* scipy

## Instructions for Reproducing the Results
To reproduce the results:
1. Install the required Python libraries: pip install pandas numpy matplotlib seaborn statsmodels scikit-learn solas-ai scipy
2. Open the Jupyter Notebook file: `RafayRaza_Assignment_3.ipynb`
3. Run all cells in the notebook from top to bottom. The notebook will:
   * Load and clean the COMPAS dataset
   * Train a logistic regression model and generate predictions
   * Compute AIR, ME, and SMD for race and sex using solas-ai
   * Confirm solas-ai results match manual calculations
   * Conduct intersectional analysis (race × sex)
   * Compute FPR and FNR by race with two-proportion z-tests
   * Produce a publication-quality bar chart of error rates by race
   * Display a compliance memo summarising all findings

The dataset is loaded directly from the ProPublica COMPAS dataset repository:  
https://raw.githubusercontent.com/propublica/compas-analysis/master/compas-scores-two-years.csv

## AI Acknowledgment
AI tools were used for general programming guidance, debugging, and assistance with Markdown formatting and grammar.
