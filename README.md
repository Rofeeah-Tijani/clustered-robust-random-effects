# Life Expectancy Analysis Using Panel Data

## 📊 Objective
To analyze how various socio-economic and health-related indicators influence **life expectancy**, while accounting for both **time** and **entity (country) effects**, and correcting for heteroscedasticity through **clustered robust standard errors**.

---

## 🧪 Methodology

- **Panel Data Structure:** Balanced panel across **193 countries** and **15 time periods**.  
- **Model Applied:** Random Effects (RE) model with **clustered robust standard errors**.

### Variables Analyzed

| Variable                  | Description |
|----------------------------|-------------|
| Sqrt_Adult_Mortality       | Square root of adult mortality rate |
| Sqrt_Infant_death          | Square root of infant death count/rate |
| Sqrt_Alcohol               | Square root of alcohol consumption |
| Sqrt_Hepatitis_B           | Square root of Hepatitis B vaccination coverage |
| Sqrt_BMI                   | Square root of Body Mass Index |
| Sqrt_Polio                 | Square root of Polio vaccination coverage |
| Sqrt_Total_Expenditure     | Square root of total health expenditure |
| Sqrt_Diphteria             | Square root of Diphtheria vaccination coverage |
| Sqrt_HIV_AIDS              | Square root of HIV/AIDS prevalence |
| Sqrt_GDP                   | Square root of GDP per capita |
| Sqrt_Schooling             | Square root of average years of schooling |

---

## 📈 Key Results

| Metric                        | Value |
|--------------------------------|-------|
| R-squared (Overall)            | 0.7555 |
| Robust F-statistic             | 96.34 (p-value: 0.0000) |
| Significance                   | Most explanatory variables significant at 1% level |
| Heteroscedasticity Adjustment  | Clustered by country to improve reliability |

**Interpretation:**  
The RE model with clustered robust standard errors confirms that **health-related expenditures, vaccination coverage, schooling, and disease prevalence** significantly influence life expectancy. Clustering by country addresses heteroscedasticity and ensures reliable statistical inference.

---

## 📌 Conclusion

- Health expenditures, disease prevention measures, and education play a **critical role in life expectancy outcomes**.  
- Robust Random Effects estimation improves the **reliability of results** under panel heteroscedasticity.  

### ✅ Recommendations

1. Invest in **education**, **healthcare access**, and **disease prevention** programs.  
2. Future studies should consider **instrumental variable techniques** to address potential endogeneity.

---

## 📁 Repository Structure

| Folder | Description |
|--------|-------------|
| `data/` | Contains cleaned panel data |
| `code/` | Python notebook with data analysis |
| `report/` | Slides and PDF report with interpretations and findings |

---

## 🔧 Tools Used

- **Python**  
  - `linearmodels` (panel data estimation)  
  - `pandas` (data manipulation)  
  - `statsmodels` (statistical inference)

---

**This repository provides a comprehensive, reproducible workflow for analyzing panel data to understand drivers of life expectancy.**
