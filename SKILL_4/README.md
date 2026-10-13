# Skill 4 — Linear Regression and Regularisation

**Project:** One Piece Bounty Prediction

## Project members
Add the team member names here if they are required for your submission.

## Contents
- `notebook/Skill_4_Reformatted.ipynb` — original notebook cells and code preserved.
- `reports/Skill_4_Lab_Record.docx` — formatted lab record with aim, apparatus/software, procedure, results, observation and conclusion.
- `reports/Skill_4_Reformatted_Report.pdf` — concise report with results and figures.
- `reports/Observation_Skill_4_Rewritten.txt` — rewritten observation in first-person student style.
- `data/` — dataset, engineered features, model metrics, coefficients, residuals and evaluation tables.
- `figures/` — supplied static figures.
- `interactive_visualizations/` — supplied HTML visualizations (open in a browser).
- `models/` — saved ElasticNet model artifact.

## Run the notebook
1. Install Python 3.10+ and Jupyter support.
2. Install the notebook dependencies if missing: `pip install pandas numpy matplotlib seaborn scikit-learn joblib`.
3. Open the notebook in VS Code or Jupyter.
4. Keep the supplied data files in the project folder or update any paths in the notebook to match your local folder structure.
5. Run the cells from top to bottom.

## Main reported result
The summary report identifies ElasticNet as the selected model (`alpha = 0.02219`, `l1_ratio = 0.99`), with test R² = 0.956 and test RMSE = 0.140 in log10 bounty units. The dataset used 142 rows. Degree 2 polynomial features were selected by Ridge cross-validation.

## Important limitation
The rank feature is derived from bounty ordering and is strongly related to the target, so it introduces target leakage. Name-only features were much weaker predictors. Treat the high test score with this limitation in mind.

## HTML visualizations
Open any file in `interactive_visualizations/` directly in a modern browser.
