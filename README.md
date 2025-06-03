📊 Objective
To analyze how various socio-economic and health-related indicators influence life expectancy, while accounting for both time and entity (country) effects, and correcting for heteroscedasticity through clustered robust standard errors.

🧪 Methodology
Panel Data Structure: Balanced panel across 193 countries and 15 time periods.

Model Applied: Random Effects (RE) model with clustered robust standard errors.

Variables Analyzed:

Sqrt_Adult_Mortality

Sqrt_Infant_death

Sqrt_Alcohol

Sqrt_Hepatitis_B

Sqrt_BMI

Sqrt_Polio

Sqrt_Total_Expenditure

Sqrt_Diphteria

Sqrt_HIV_AIDS

Sqrt_GDP

Sqrt_Schooling

📈 Key Results
R-squared (Overall): 0.7555

Robust F-statistic: 96.34 (p-value: 0.0000)

Most explanatory variables are statistically significant at the 1% level.

Clustering by country addresses heteroscedasticity and improves reliability of inference.

📌 Conclusion
The analysis shows that health-related expenditures, vaccination coverage, schooling, and disease prevalence significantly impact life expectancy. The use of robust RE estimation enhances model reliability under panel heteroscedasticity.

✅ Recommendation
Invest in education, healthcare access, and disease prevention to improve life expectancy.

Future studies should consider instrumental variable techniques to address potential endogeneity.

📁 Files
data/ – Contains cleaned panel data.

code/ – Python notebook for data analysis.

report/ – Slides and PDF report with interpretations and findings.

🔧 Tools Used
Python (linearmodels, pandas, statsmodels)

Jupyter Notebook



