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

