# IH-DA-Project02

# Vanguard A/B Test Project

## Overview
This project analyzes the impact of a redesigned digital interface for Vanguard’s clients through a controlled A/B test. The goal was to determine if a more modern and intuitive digital design, with contextual prompts, led to improved client completion rates in an online process compared to the traditional user interface.

The analysis encompasses end-to-end data preparation, exploratory data analysis (EDA), KPI definition, hypothesis testing, experiment evaluation, and dashboard/storytelling development using Tableau.

## Repository Structure
🔹 vanguard-ab-test/
🔹 data/               # Raw datasets
🔹 notebooks/          # Jupyter notebooks for EDA, metrics, hypothesis testing
🔹 scripts/            # Python scripts for reusable functions
🔹 tableau/            # Packaged Tableau workbook (.twbx)
🔹 slides/             # Final project presentation
🔹 README.md           # Project overview
🔹 requirements.txt    # Project dependencies
🔹 .gitignore          # Files/folders to be ignored by Git


## Project Deliverables
### EDA and Data Cleaning
- Merged the **Client Profiles**, **Web Activity Logs (pt1 and pt2)**, and **Experiment Assignment** datasets using `client_id`.
- Handled missing values, duplicates, and inconsistent formats (e.g., corrected date formats, cleaned demographic data).
- Engineered new features such as tenure in months/years, number of steps completed, and completion flags.

### Client Behavior Analysis
- Analyzed client interactions across steps (Initial Page, Step 1, Step 2, Step 3, Confirmation Page).
- Identified drop-off points and compared user journeys between Test and Control groups.

### Performance Metrics Definition
- Calculated KPIs including:
  - **Completion Rate** (percentage reaching the final confirmation step)
  - **Error Rate** (sessions with missing or inconsistent steps)
  - **Average Time Per Step**
  - **Number of Actions** performed

### Hypothesis Testing and Experiment Evaluation
- Conducted hypothesis testing to determine whether the Test group’s completion rate was statistically higher.
- Carried out cost-effectiveness analysis considering operational costs versus completion improvements.
- Evaluated experimental design (random assignment, sample size sufficiency, and data fairness).

### Tableau Visualization and Dashboarding
- Created a **Choropleth Map** to show client distribution by State.
- Built a **Regression Plot** analyzing the relationship between Customer Lifetime Value and Income.
- Created a **Boxplot** to visualize Total Claim Amount distribution by Vehicle Size.
- Developed a **Dashboard** combining all key visualizations.
- Designed a **Story** presenting the experiment results step-by-step.

### Final Presentation
- Compiled all insights, data challenges, experiment evaluations, and visual stories into a professional presentation.


## Tools Used
- Python (Pandas, NumPy, SciPy, Statsmodels)
- Jupyter Notebook
- Tableau Public/Desktop
- Trello (Kanban Board for project management)
- Git & GitHub for version control and collaboration


## Data Sources
- **Client Profiles (df_final_demo.csv)**: Client ID, tenure, age, gender, account details.
- **Web Activity Logs (df_final_web_data_pt1.csv and df_final_web_data_pt2.csv)**: Digital footprints recording process steps, timestamps, and session details.
- **Experiment Assignment (df_final_experiment_clients.csv)**: Grouping information identifying Control and Test group clients.

Each record includes important metadata:
- `client_id`, `variation`, `visitor_id`, `visit_id`, `process_step`, `date_time`, `clnt_tenure_yr`, `clnt_age`, `gendr`, `num_accts`, `bal`, `calls_6_mnth`, `logons_6_mnth`
## How to Run
1. Clone the repository:
    ```bash
    git clone https://github.com/10197jsg/IH-DA-Project02.git
    cd IH-DA-Project02
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebooks inside `/notebooks/` for data processing and analysis.
4. Open the Tableau workbook `tableau_file.twbx` in Tableau Public/Desktop to view dashboards and story.

## Links
- **Trello Board**: [Trello Board Invitation](https://trello.com/invite/b/67f1218020a62270e1df760c/ATTIc3df754809889611cb5d2965820dc7e8777E2D52/house-baratheon-project-2)
- **Project Presentation**: [https://prezi.com/p/edit/wtzwcmra1tlx/]
- **Tableau Workbook**: [Tableau Workbook](https://public.tableau.com/views/baratheon_tableau_file/ABTesting?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
- **Repository**: [GitHub Repository](https://github.com/10197jsg/IH-DA-Project02)


## Authors
- Germán Álvarez [https://github.com/german-alvarez-dev]
- Hilena Amare Tadesse [https://github.com/hilu1]
- Ahmad Khalil Ghamai [https://github.com/ahmad2025-ai]
- Jud Saavedra [https://github.com/10197jsg]


## Additional Notes
- Bonus analyses performed include client navigation pattern analysis and post-hoc power analysis.
- Streamlit was explored for future interactive visualizations.

