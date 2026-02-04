# Trader Performance vs Market Sentiment

This repository contains my submission for the **Data Science Intern – Round 0 Assignment**.  
The objective of this project is to analyze how **Bitcoin market sentiment (Fear vs Greed)** impacts
**trader performance and behavior** on the Hyperliquid platform, and to derive
**actionable trading insights** supported by data.

---

## 📁 Project Structure

assignment/
│
├── analysis.ipynb # Main notebook (data prep, analysis, insights)
├── README.md # Setup, execution, and project summary
├── insights.txt # Short write-up (methodology, insights, strategies)
├── requirements.txt # Python dependencies
│
├── data/
│ ├── fear_greed_index.csv
│ └── historical_data.csv
│
└── charts/ # Output charts & tables
├── insight1_pnl_distribution.png
├── insight1_pnl_table.csv
├── insight2_behavior_table.csv
├── insight2_trade_frequency.png
├── insight3_bias_table.csv
└── insight3_long_bias.png


---

## ⚙️ Setup Instructions

### 1️ Clone the repository
```bash
git clone <your-github-repo-link>
cd assignment
2️ (Optional but recommended) Create virtual environment
python -m venv venv
Activate it:

Windows

venv\Scripts\activate
Mac / Linux

source venv/bin/activate
3️ Install dependencies
pip install -r requirements.txt
▶️ How to Run
Option 1: Run the Notebook (Preferred)
jupyter notebook
Open analysis.ipynb and run all cells top to bottom.

This will:

Load and clean the datasets

Aggregate trades at a daily trader level

Align trader metrics with Fear/Greed sentiment

Generate summary tables in the notebook

Save output charts and tables in the charts/ directory

 Output Artifacts
Tables
Displayed directly in the notebook and saved as CSV files in charts/

Charts
Saved as PNG files in the charts/ directory for reproducibility

These outputs provide evidence-backed insights for all conclusions.

 Analysis Summary (Short Write-up)
A concise write-up covering methodology, key insights, and strategy recommendations
is provided in insights.txt, as required by the assignment.

 Requirements
All required libraries are listed in requirements.txt, including:

pandas

numpy

matplotlib

seaborn
