# Greedy Cloud Latency — ML Project

This repository analyzes latency variations across different cloud providers and geographic regions using machine learning.
It includes an exploratory notebook and a written report for recruiters and reviewers.

## Repo Contents
- `gmcsd_new.ipynb` — Jupyter notebook with the full analysis and experiments
- `report/annotated-ML_Report.pdf` — Final report with methodology and results
- `requirements.txt` — Python dependencies to run the notebook
- `data/` — (empty) place sample data here if needed (do not commit large/private datasets)

## Dataset
Public dataset: Greedy Cloud Selection Deployment on Microservices (Kaggle)  
https://www.kaggle.com/datasets/nickkinyae/greedy-cloud-selection-deployment-on-microservices

> NOTE: Large datasets should not be committed. Link to the source instead.

## How to Run Locally
```bash
# 1) Create a virtual environment (optional but recommended)
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

# 2) Install dependencies
pip install -r requirements.txt

# 3) Launch Jupyter
jupyter notebook gmcsd_new.ipynb
```

## Methods Tried (high level)
- Data cleaning, encoding of categorical features, normalization
- Outlier detection and correlation analysis
- Baselines and tree-based models (DecisionTree, RandomForest)
- Attempted polynomial feature expansion

**Observation:** The dataset showed weak direct correlation with latency; models tended to overfit and did not generalize well. See the PDF report for details and discussion.

## Project Structure
```
greedy-cloud-latency-ml/
├── README.md
├── requirements.txt
├── gmcsd_new.ipynb
├── report/
│   └── annotated-ML_Report.pdf
└── data/
    └── .gitkeep
```

