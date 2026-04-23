# ACC102 individual assignment
Project Title: ESG Scores and Stock Market Preformance Analysis
# 1.Problem & User
* This project examines whether corporate ESG performance correlates with stock returns and volatility, to identify risk and return patterns across different sustainability tiers. 
* The analysis is designed to support hypothetical investors or financial analysts who wish to understand how ESG scores relate to real-world stock performance.
# 2.Data
1. ESG Data: Local CSV file (esg_return_sample.csv), accessed April 2026. Key fields: permno, esg_score, volatility.
2. Return Data: Monthly stock returns from WRDS CRSP database (Jan 2023–Dec 2024), accessed April 22, 2026. Key fields: permno, date, ret.
* Datasets merged on permno identifiers for 1-to-1 matching.
# 3.Methods
1. Load ESG data and extract company identifiers
2. Download stock returns from WRDS using SQL
3. Aggregate monthly returns to annual average return and volatility
4. Merge datasets and classify ESG into three equal groups
5. Generate 4 visualizations and auto-save figures
6. Output analysis summary
# 4.Key Findings
1. Medium ESG group has the highest average return
2. Positive correlation between ESG and returns
3. Strong negative correlation between ESG and volatility
4. Higher ESG = lower risk
# 5.How to Run
1. Place "esg_return_sample.csv" and "ESG_Analysis.ipynb" in the same folder
2. Install required packages: pandas, numpy, matplotlib, seaborn, wrds
3. Run the Python script
* Figures will be automatically saved to the folder, and a summary report will print to the console.
# 6.Limitations & Next Steps
1. Small sample and short time window
2. No industry or firm-size controls
3. Static ESG scores only
* Next steps: expand data, add industry controls, use dynamic ESG data
