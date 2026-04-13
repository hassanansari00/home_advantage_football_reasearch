# Quantifying the Home-Field Advantage in the English Premier League ⚽📊

**Author:** [HASSAN ANSARI]  
**Objective:** Independent Data Science Research Project (BSc Data Science Application)

## 📌 Project Overview
This project investigates the mathematical validity of the "Home-Field Advantage" phenomenon in professional football. Moving beyond subjective fan theories, this analysis uses Python to process raw match-day data from the 2023/2024 English Premier League season to quantify the exact impact of stadium location on team attacking efficiency and disciplinary metrics.

## 🛠️ Tools & Technologies Used
* **Language:** Python 3
* **Libraries:** * `pandas` (Data Engineering, Cleaning, and Aggregation)
  * `matplotlib` & `seaborn` (Data Visualization)
* **Environment:** Jupyter Notebook / Google Colab

## 🗄️ Data Sourcing & Engineering
The raw dataset contains match-by-match results for the complete 23/24 Premier League season. Before analysis, data engineering was required to make the dataset readable and usable:
1. **Data Filtering:** The original dataset contained over 100 columns, including betting odds and irrelevant noise. I used Python (`pandas`) to slice the dataframe, isolating only the core match statistics needed for this study.
2. **Data Standardization:** The raw data used confusing, abbreviated column headers (e.g., `FTHG` for Full Time Home Goals, `HY` for Home Yellows). I wrote a dictionary mapping to rename these variables into standardized, plain-English categories (e.g., `Home_Goals`, `Home_Yellows`) to ensure the final analysis was transparent and easily interpretable by any stakeholder.

## 📈 Key Findings
Through Exploratory Data Analysis (EDA) of the dataset, I analyzed three core metrics to prove the home advantage:

1. **Offensive Output (Goals):** The data mathematically proves a **21.6% goal-scoring advantage** simply for playing at a home venue (averaging 1.80 home goals vs. 1.48 away goals per match).
2. **Attacking Pressure (Shots on Target):** Home teams consistently generated a higher volume of shots on target per match, proving the goal advantage is driven by systematic attacking pressure rather than mere finishing luck.
3. **Disciplinary Bias (Yellow Cards):** Away teams received a higher average of yellow cards per match, indicating that playing in front of an opposing crowd correlates with more aggressive defensive errors or stricter officiating.

## 🚀 How to Run the Project
1. Clone this repository to your local machine.
2. Ensure you have Python installed along with `pandas`, `matplotlib`, and `seaborn`.
3. Open the `homeadvantage research.ipynb` file in Jupyter or upload it to Google Colab.
4. Ensure the `PL 2023-24.csv` dataset is located in the same directory.
5. Run all cells to reproduce the data cleaning process and view the final statistical outputs and visualizations.

## 🔭 Future Scope
For future iterations of this project, I plan to integrate advanced underlying metrics, such as **Expected Goals (xG)** and **Possession Statistics**, to determine if the home advantage is driven by genuine tactical dominance and chance creation or higher finishing variance.
