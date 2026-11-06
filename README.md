# CISC7204-ClassF-Group04-Project
Final project for CISC7204 (Team4 Group 04)
## 📌 Project Title
**Multi-Sport Comparison of Athlete Injury Risks: A Clinical Biomechanics and Training Load Analysis**

## 👥 Group Members
| Name | Student ID |
| :--- | :--- |
| Li Ke Xin | mc662930 |
| Fu Yu Xin | MC663207 |
| Shi Yue Tong | mc662092 |
| He Ying Tong | MC660441 |
| Tao Ao Ran | MC663520 |
| Wu Dan | mc662342 |

## 📖 Project Overview
This project investigates whether different sports exhibit statistically significant differences in severe injury risks, and how training load and fatigue mediate these differences. We utilize a primary clinical dataset (15,000 records, 10 sports) and two external datasets for validation.

## 📂 Repository Structure
- `notebooks/`: The main reproducible Jupyter Notebook.
- `data/`: The primary and external datasets used.
- `figures/`: All 7 publication-ready data visualizations generated from the analysis.
- `report/`: The final compiled PDF report.

## 🛠️ How to Run
All analyses were conducted in Python 3.x. To reproduce the results:
1. Ensure you have installed the required libraries: `pip install pandas numpy scipy statsmodels seaborn matplotlib`
2. Open `notebooks/Group04_Analysis.ipynb` in Jupyter Notebook.
3. The notebook uses relative paths. Simply click **"Run All"** to execute the entire pipeline from data loading to visualization.

## 📊 Key Findings
1. **Baseline Risk:** Critical injury risk is relatively uniform across all 10 sports (overlapping 95% Wilson CIs).
2. **Core Predictors:** After adjusting for confounders via multivariate logistic regression, `workload_ratio` (Adjusted OR ≈ 6.0) and `previous_injury_history` (Adjusted OR ≈ 1.9) are the dominant risk factors.
3. **Sport Type:** `sport_type` is not a statistically significant independent predictor once training load and fatigue are accounted for.
4. **External Validation:** External datasets confirmed the validity of training load metrics and the consistent doubling of risk associated with prior injury history (OR = 2.04, p < 0.001).
