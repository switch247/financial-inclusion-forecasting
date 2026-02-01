# Ethiopia Financial Inclusion Forecasting

Professional-grade repository for the Week 10 challenge: forecasting Ethiopia's financial inclusion indicators and modelling event impacts.

Business objective
- Build a forecasting system that predicts two Global Findex indicators for Ethiopia and quantifies how events (policy, product launches, infrastructure) affect those indicators:
  - Access — Account Ownership Rate (% adults with an account or using mobile money)
  - Usage — Digital Payment Adoption Rate (% adults who made/received a digital payment)

Scope and deliverables
- Enriched, unified dataset and a data-enrichment log.
- Exploratory data analysis with visualizations and written insights.
- Event–indicator association matrix and impact-modeling notebook.
- Scenario forecasts (baseline / optimistic / pessimistic) for 2025–2027 with uncertainty estimates.
- Interactive Streamlit dashboard (`dashboard/app.py`) to explore data, events, and forecasts.

Status (high level)
- Data ingestion & repository scaffold: ready.
- Task 1 (Data enrichment): branch `task-1` recommended.
- Task 2 (EDA): notebooks scaffolded in `notebooks/` (work in progress).
- Task 3–5 (impact modeling, forecasting, dashboard): planned; see `experiments/todo.md` for task-level checklists and timelines.

Repository layout
```
<project root>
├── dashboard/                # Streamlit app and static assets
├── data/
│   ├── raw/                  # Raw inputs (starter datasets, reference codes)
│   └── processed/            # Enriched and analysis-ready datasets
├── docs/                     # Documentation and guides
├── experiments/              # Challenge brief and local experiment notes
├── notebooks/                # EDA, impact-modeling, forecasting notebooks
├── outputs/                  # Generated figures, models, reports
├── scripts/                  # Utilities and pipeline helpers
├── src/                      # Reusable modules and modeling code
├── tests/                    # Unit tests
├── requirements.txt          # Python dependencies
└── README.md                 # This file
```

Note about tracked vs ignored items
Some local files and folders (for example large CSVs, outputs, and experiment scratch files) may be excluded from version control via `.gitignore`. Check `.gitignore` before creating or relying on files that need sharing or CI-based runs.

Quick start
1. Create and activate a virtual environment and install dependencies:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

2. Run EDA and model notebooks in `notebooks/` using Jupyter or VS Code.

3. Launch the dashboard locally:

```powershell
streamlit run dashboard/app.py
```

Recommended workflow
- Create a feature branch named for the task (e.g., `task-1`, `task-2`).
- Keep raw data changes and enrichment logs under `data/` and record additions in `data/data_enrichment_log.md`.
- Push small, focused commits and open PRs for review.

Contribution and licensing
- Follow the repository coding conventions; place reusable code in `src/` and keep notebooks for exploration.
- Add unit tests for any production code in `src/` under `tests/`.

References
- See `experiments/todo.md` for the full challenge brief, task checklists, timelines, and references.

Contact
- For questions about tasks or submissions, coordinate via the project channel or the challenge tutors listed in `experiments/todo.md`.

