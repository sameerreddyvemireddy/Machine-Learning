# Skill 5 — Logistic Regression Classification

## Project overview
This package contains the Skill 5 notebook, One Piece bounty data, the supplied saved Logistic Regression model, evaluation/report files, interactive HTML dashboards, and figures for exploratory analysis and classification evaluation.

## Package structure
- `notebook/Skill_5.ipynb` — original notebook, code preserved
- `data/` — source CSV, provided result tables, and recreated feature table
- `model/onepiece_logistic_regression.joblib` — supplied serialized model
- `figures/` — PNG figures generated from the uploaded dataset and documented evaluation metrics
- `interactive/` — provided Plotly HTML dashboards
- `reports/` — supplied reports and rewritten observation

## Reported project setup
The supplied report identifies a `StandardScaler + LogisticRegression` pipeline. It reports 165 raw records, 144 usable Berry records, and a high-bounty threshold of 332,500,000 Berries. Reported held-out metrics: accuracy 0.7241, precision 0.4286, recall 0.4286, F1 0.4286, ROC AUC 0.6364, average precision 0.6082, and log loss 0.5372. These are reproduced from the supplied report, not recalculated from the notebook.

## Run in VS Code
1. Extract the ZIP and open this folder in VS Code.
2. Install Python 3.10+ and the Jupyter extension.
3. Create/activate a virtual environment.
4. Install common notebook dependencies: `pip install pandas numpy matplotlib scikit-learn joblib jupyter`.
5. Open `notebook/Skill_5.ipynb` and run cells in order.

The original notebook may expect files at its original relative paths. If so, copy the required CSV from `data/` to the path referenced in the notebook, or update the data path only (do not alter model logic). Loading a `.joblib` file requires a compatible scikit-learn version with the one used when it was saved. Only load trusted serialized model files.

## Figures and interpretation
The `figures/` PNGs are recreated from the uploaded source CSV and report values. Since the supplied raw CSV may include non-numeric or unknown bounty formats, counts in recreated figures can differ from the documented analysis if parsing rules differ. The report's documented counts and metrics are preserved as reported. Correlation is descriptive and does not imply causation.
