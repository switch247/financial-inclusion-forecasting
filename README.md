# Ethiopia Financial Inclusion Forecasting

Professional-grade repository for the Week 10 challenge: forecasting Ethiopia's financial inclusion indicators and modelling event impacts.

## Business Objective
- Build a forecasting system that predicts two Global Findex indicators for Ethiopia and quantifies how events (policy, product launches, infrastructure) affect those indicators:
  - **Access** — Account Ownership Rate (% adults with an account or using mobile money)
  - **Usage** — Digital Payment Adoption Rate (% adults who made/received a digital payment)

## Scope and Deliverables
- **Task 1: Data Exploration and Enrichment** - Explicitly load and document understanding of `ethiopia_fi_unified_data.csv` unified schema, enrich with additional observations, events, and impact links for comprehensive analysis.
- **Task 2: Exploratory Data Analysis (EDA)** - Plot 2011–2024 access/usage trajectories, deeply analyze 2021–2024 slowdown with overlaid event timelines, and provide at least five numbered key insights tying data patterns to events and policy context.
- **Task 3: Event Impact Modeling** - Event–indicator association matrix and impact-modeling notebook.
- **Task 4: Forecasting Access and Usage** - Scenario forecasts (baseline / optimistic / pessimistic) for 2025–2027 with uncertainty estimates.
- **Task 5: Dashboard Development** - Interactive Streamlit dashboard to explore data, events, and forecasts.

## Status
✅ **All Tasks Completed**
- Task 1: Data enrichment completed with unified schema documentation and enriched dataset (`data/processed/ethiopia_fi_unified_data_enriched.csv` with 49 records including events and impact links)
- Task 2: EDA completed with explicit 2011-2024 access/usage trajectories, deep 2021-2024 slowdown analysis, event-overlaid timelines, and 5+ numbered key insights in `notebooks/02_eda.ipynb`
- Task 3: Event impact modeling completed with association matrix (4x3), validation, documentation in `notebooks/03_event_impact_modeling.ipynb`
- Task 4: Forecasting completed with trend models, scenarios, uncertainty quantification in `notebooks/04_forecasting_access_usage.ipynb`
- Task 5: Interactive dashboard implemented with 4 pages, data downloads, and visualizations in `src/dashboard/app.py`

## Repository Layout
```
<project root>
├── data/
│   ├── raw/                  # Raw inputs (starter datasets, reference codes)
│   └── processed/            # Enriched and analysis-ready datasets
├── docs/                     # Documentation and guides
├── experiments/              # Challenge brief and local experiment notes
├── notebooks/                # EDA, impact-modeling, forecasting notebooks
├── outputs/                  # Generated figures, models, reports, CSVs
├── scripts/                  # Utilities and pipeline helpers
├── src/
│   ├── dashboard/            # Streamlit app
│   └── utils/                # Reusable modules (plotter, data loaders, etc.)
├── tests/                    # Unit tests
├── requirements.txt          # Python dependencies
└── README.md                 # This file
```

## Key Outputs
- **Data**: Enriched dataset with 49 records including events and impact links
- **Analysis**: Event-indicator matrix (4x3), correlation analysis, temporal trends
- **Forecasts**: 2025-2027 projections with baseline/optimistic/pessimistic scenarios
- **Visualizations**: Interactive charts using Plotly, saved figures in `outputs/figures/`
- **Dashboard**: 4-page Streamlit app with data exploration and forecast visualization

## Quick Start
1. **Setup Environment**:
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   pip install -r requirements.txt
   ```

2. **Run Notebooks**:
   - Open and run analysis notebooks in `notebooks/` using Jupyter or VS Code
   - Notebooks include: EDA, event modeling, forecasting

3. **Launch Dashboard**:
   ```powershell
   streamlit run src/dashboard/app.py
   ```
   Access at http://localhost:8501 for interactive exploration

## Workflow and Best Practices
- All analysis uses the custom `Plotter` utility for consistent visualizations
- Data processing follows the pipeline in `scripts/pipeline.py`
- Outputs are saved to `outputs/` directory with auto-generated figures
- Unit tests available in `tests/` for core utilities

## Dependencies
- Python 3.11+
- Key libraries: pandas, numpy, scikit-learn, statsmodels, plotly, streamlit
- See `requirements.txt` for full list

## References
- Challenge brief and task details: `experiments/todo.md`
- Business understanding: `docs/business_understanding.md`
- Data dependencies: `docs/dependencies.md`

## Contact
- For questions about implementation or results, refer to notebook outputs and dashboard

