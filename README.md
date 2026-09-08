# Manufacturing Data Integration & Operational Analysis

This project integrates machine operating data, supplier characteristics, production-batch information, and product test results to investigate patterns associated with manufacturing performance.

The analysis compares production behavior across machines, suppliers, and batches, then uses unsupervised clustering to identify operating-condition profiles associated with substantially different product failure rates.

## Project Objective

The objective is to combine multiple manufacturing data sources into a unified analytical dataset and determine which production characteristics are most strongly associated with differences in product test outcomes.

## Data

The analysis uses five source datasets:

- Three machine datasets containing production-batch and operating measurements (`x1`, `x2`, `x3`, and `x4`)
- Supplier data containing supplier and material-density information for each production batch
- Product test results containing pass/fail outcomes for tested products

The datasets are integrated using production batch and individual product identifiers.

> **Data availability:** The source CSV files were provided as part of academic coursework and are not included in this public repository unless redistribution permission is confirmed.

## Tools & Methods

**Python • Pandas • Matplotlib • Seaborn • scikit-learn • KMeans Clustering**

Methods include:

- Data integration and validation
- Exploratory data analysis
- Distribution and correlation analysis
- Failure-rate analysis
- Feature standardization
- KMeans clustering
- Inertia and silhouette analysis

## Key Findings

- Machine failure rates were relatively similar, ranging from 67.7% to 72.2%.
- Supplier B had a higher failure rate than Supplier A despite producing fewer failures in absolute terms.
- Production batches showed substantial variation in test outcomes, with observed failure rates ranging from 0% to 100%.
- Eight operating-condition clusters were identified using KMeans.
- Cluster failure rates ranged from 3.5% to 94.6%, indicating a strong association between combinations of operating conditions and product test outcomes.

These findings are observational. Additional controlled analysis would be required before treating the relationships as causal or using them to establish production settings.

## Repository Contents

- `manufacturing_analysis.ipynb` — complete analysis notebook
- `manufacturing_analysis.html` — read-only exported analysis
- `README.md` — project overview and findings
- `requirements.txt` — Python package dependencies
- `DATA_NOTE.md` — source-data availability note

## Author

**Lynn Ruch**  
M.S. Data Science Candidate, University of Pittsburgh
