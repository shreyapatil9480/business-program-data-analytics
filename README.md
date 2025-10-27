
# Business, Program, and Data Analytics Project

This repository contains a synthetic dataset and analysis notebook designed to showcase skills relevant to business analysts, program managers, and data analysts. The project demonstrates how to generate insights from project management data, visualize relationships, and build predictive models to anticipate project success.

## Project Overview

Organizations often manage multiple projects concurrently, and understanding which factors lead to project success can help allocate resources more effectively. This project includes:

- **Synthetic dataset (`project_dataset.csv`)** containing 300 projects with attributes such as start/end dates, budget, actual spending, complexity, team size, scope changes, quality score, and success outcome.
- **Jupyter notebook (`analysis.ipynb`)** performing exploratory data analysis (EDA), visualizations, and building logistic regression and random forest models to predict project success.
- **Requirements file (`requirements.txt`)** listing Python packages needed to run the notebook.

## Dataset Description

The dataset is stored in `data/project_dataset.csv`. Each row represents one project with the following columns:

| Column | Description |
|-------|-------------|
| `project_id` | Unique project identifier |
| `start_date` | Project start date |
| `end_date` | Project end date |
| `duration_days` | Number of days from start to end |
| `budget` | Planned budget in USD |
| `spent_amount` | Actual spending in USD |
| `complexity` | Project complexity category (Low, Medium, High) |
| `team_size` | Number of people on the project team |
| `scope_changes` | Count of significant scope changes |
| `quality_score` | Final quality score (0–100) |
| `success` | Indicator (0 or 1) of whether the project was considered successful |

All values are randomly generated but reflect realistic ranges and relationships.

## Getting Started

1. **Clone the repository** (or download as ZIP) and navigate into the folder.

2. **Set up a virtual environment** (optional but recommended):

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate  # On Windows use: .venv\Scriptsctivate
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Open the notebook**:

   ```bash
   jupyter notebook notebooks/analysis.ipynb
   ```

5. **Run the notebook cells** to reproduce the analysis, generate plots, and view model results. Feel free to experiment with different model parameters or add additional analyses.

## Extending the Project

- **Feature Engineering**: Try creating new features such as spent ratio (spent_amount / budget) or schedule variance.
- **Model Tuning**: Adjust hyperparameters of the random forest or experiment with other algorithms like gradient boosting or support vector machines.
- **Real Data**: Replace the synthetic dataset with real project management data from your organization (ensuring you have permission and anonymizing sensitive information).
- **Dashboards**: Build interactive dashboards (using tools like Tableau, Power BI, or Python libraries such as Plotly Dash) to visualize project performance metrics.

## License

This project is provided for educational purposes and does not include a license. Feel free to use and modify the code for personal or professional learning.
