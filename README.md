# IH-DA-Project02

# Vanguard A/B Test Project

## Overview
This project analyzes the impact of a redesigned digital interface for Vanguard’s clients through a controlled A/B test. The goal was to determine if a more modern and intuitive digital design, with contextual prompts, led to improved client completion rates in an online process compared to the traditional user interface.

The analysis encompasses end-to-end data preparation, exploratory data analysis (EDA), KPI definition, hypothesis testing, experiment evaluation, and dashboard/storytelling development using Tableau.

---

## Repository Structure
```
vanguard-ab-test/
🔹 data/               # Raw datasets
🔹 notebooks/          # Jupyter notebooks for EDA, metrics, hypothesis testing
🔹 scripts/            # Python scripts for reusable functions
🔹 tableau/            # Packaged Tableau workbook (.twbx)
🔹 slides/             # Final project presentation
🔹 README.md           # Project overview
🔹 requirements.txt    # Project dependencies
🔹 .gitignore          # Files/folders to be ignored by Git
```

---

## Project Deliverables
- **EDA and Data Cleaning**
  - Merging client profile and web interaction datasets.
  - Handling missing values, duplicates, and inconsistent formatting.
- **Performance Metrics Definition**
  - Key metrics such as Completion Rates, Error Rates, and Average Time per Step.
- **Hypothesis Testing and Experiment Evaluation**
  - Hypothesis testing to assess the significance of improved completion rates.
  - Evaluation of experiment design, sample size sufficiency, and potential biases.
- **Tableau Dashboards and Story Creation**
  - Visual storytelling of the A/B test results.
  - Dynamic filtering by demographics (age, gender).
- **Final Project Presentation**
  - Insights, recommendations, and a detailed evaluation of experiment outcomes.

---

## Tools Used
- Python (Pandas, NumPy, SciPy, Statsmodels)
- Jupyter Notebook
- Tableau Public/Desktop
- Trello (Kanban Board for project management)
- Git & GitHub for version control and collaboration

---

## Data Sources
- **Client Profiles (df_final_demo.csv)**: Client ID, tenure, age, gender, account details.
- **Web Activity Logs (df_final_web_data_pt1.csv and df_final_web_data_pt2.csv)**: Digital footprints recording process steps, timestamps, and session details.
- **Experiment Assignment (df_final_experiment_clients.csv)**: Grouping information identifying Control and Test group clients.

Each record includes important metadata:
- `client_id`, `variation`, `visitor_id`, `visit_id`, `process_step`, `date_time`, `clnt_tenure_yr`, `clnt_age`, `gendr`, `num_accts`, `bal`, `calls_6_mnth`, `logons_6_mnth`

---

## How to Run
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/vanguard-ab-test.git
    cd vanguard-ab-test
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebooks inside `/notebooks/` for data processing and analysis.
4. Open the Tableau workbook `vanguard-dashboard.twbx` in Tableau Public/Desktop to view dashboards and story.

---

## Links
- **Trello Board**: [Trello Board Invitation](https://trello.com/invite/b/67f1218020a62270e1df760c/ATTIc3df754809889611cb5d2965820dc7e8777E2D52/house-baratheon-project-2)
- **Project Presentation**: [Project Presentation](https://dataptjan14th2025.slack.com/archives/C08LZ2PVCKE/p1745074682042689)
- **Tableau Workbook**: [Tableau Workbook](https://dataptjan14th2025.slack.com/archives/C08LZ2PVCKE/p1745074682042689)
- **Repository**: [GitHub Repository](https://github.com/10197jsg/IH-DA-Project02)

---

## Authors
- Hilena Amare Tadesse
- [Partner Name if applicable]

---

## Additional Notes
- Bonus analyses performed include client navigation pattern analysis and post-hoc power analysis.
- Streamlit was explored for future interactive visualizations.

---
