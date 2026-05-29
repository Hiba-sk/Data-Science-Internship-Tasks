# 🤖 AI Mental Health Assistance

A professional NHS-aligned data science pipeline for mental health analytics. This project covers the full lifecycle from raw data ingestion and schema mapping to machine learning, time-series forecasting, and clinical decision support.

📌 **Project Focus:** Transitioning the Trust from reactive reporting to proactive operational modeling using MHSDS and Prescribing datasets.


## 📁 Project Structure

```text
AI-Mental-health-Assistance-/
│
├── datasets/                   # Raw NHS CSVs (ASCOF, IAPT, Prescribing)
├── outputs/                    # Generated visuals (Charts, Maps, Logs)
│   ├── mhsds_pipeline_volume_totals.png
│   ├── demo_clustering_outliers.png
│   └── demo_forecast_radar.png
│
├── scripts/
│   ├── week1/                  # Statistical Foundations
│   ├── week2/                  # ML & Clustering
│   ├── week3/                  # Forecasting & Spatial
│   └── week4/                  
│       ├── mhsds_pipeline_module.py    # Automated monthly append engine
│       └── demo_outputs.py             # Clinical demo visualization suite
│
├── reports/                    # Methodology & Compliance Documentation
│   ├── NHS_Methodology_Compliance_Note.pdf
│   └── Clinical_Demo_Narrative.md
│
├── run_all.py                  # Master pipeline runner
├── mhsds_master_historical.csv # The unified production dataset
├── requirements.txt
└── README.md
```

## ⚙️ Installation

### Prerequisites
*   **Python 3.8+**
*   **Git** (installed and configured)
    ```

2.  **Create and Activate a Virtual Environment:**
    *   **Windows:**
```bash
        python -m venv venv
        .\venv\Scripts\activate
```
    *   **macOS/Linux:**
```bash
        python3 -m venv venv
        source venv/bin/activate
```

3.  **Install Core and Specialized Dependencies:**
```bash
    pip install --upgrade pip
    pip install -r requirements.txt
```

## 🚀 Running the Pipeline

### 1. End-to-End Orchestration
To execute the master analytics runner across all chronological sprint directories:
```bash
python run_all.py

```

## 📂 Dependencies

The pipeline requires the following Python libraries for data processing, modeling, and visualization:

| Package | Purpose |
| :--- | :--- |
| `numpy` / `pandas` | High-performance data manipulation and cleaning. |
| `scipy` / `statsmodels` | Advanced statistical analysis and hypothesis testing. |
| `scikit-learn` | Machine learning (Clustering & Anomaly Detection). |
| `prophet` | Robust time-series forecasting for clinical demand. |
| `matplotlib` / `seaborn` | High-fidelity data visualization and clinical charting. |
| `geopandas` | Geospatial mapping and health inequality analysis. |
| `openpyxl` / `xlrd` | Handling of historical NHS Excel data formats. |

**Install all dependencies at once:**
```bash
pip install -r requirements.txt

```

## 📊 Outputs

All generated outputs are saved to the `outputs/` directory, including:
* **Statistical Analysis:** Test results, p-values, and summary tables.
* **Regression Models:** Performance metrics (MAE, RMSE) for secondary-use data.
* **Patient Clustering:** Multi-dimensional visualisations of service segments.
* **Demand Forecasts:** Longitudinal IAPT/MHSDS charts with confidence intervals.
* **Anomaly Reports:** Flagged prescribing variances and potential clinical outliers.
* **Geospatial Maps:** Heatmaps of service access vs. deprivation indices.
* **Pipeline Logs:** Full pipeline run logs (idempotency and validation checks).

---

## 📝 Reports

Detailed written reports for each analysis phase are available in the `Reports/` directory:
* `Week 1 : Statistical_Foundations_Report.pdf`
* `Week 2 : ML_Clustering_Report.pdf`
* `Week 3 : Forecasting_Geospatial_Impact.pdf`
* `Week 4 : NHS_Methodology_Compliance_Note.pdf` (Final IG/Clinical Audit Document)

---

## ⚠️ Data Note

This project uses NHS mental health service datasets. Ensure any data placed in `datasets/` complies with applicable data governance, UK GDPR protocols, and NHS data sharing agreements before use. All data used in this pipeline is aggregated to ensure patient anonymity.

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.
