# Trader Performance vs Market Sentiment

This repository contains my submission for the **Data Science Intern – Round 0 Assignment**.  
The objective of this project is to analyze how **Bitcoin market sentiment (Fear vs Greed)**
impacts **trader performance and behavior** on the Hyperliquid platform and to derive
**actionable trading insights** supported by data.

---

## 📁 Project Structure

assignment/
│
├── analysis.ipynb # Main notebook (data prep, analysis, insights)
├── README.md # Project overview, setup, and execution steps
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

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Abhilashaaaaaa13/assignment.git
cd assignment

2️⃣ (Optional but recommended) Create a virtual environment
python -m venv venv


Activate it:

Windows

venv\Scripts\activate


Mac / Linux

source venv/bin/activate

3️⃣ Install dependencies
pip install -r requirements.txt

▶️ How to Run the Analysis
Option 1: Run the Notebook (Preferred)
jupyter notebook


Open analysis.ipynb and run all cells top to bottom.

This will:

Load and clean both datasets

Aggregate trades at a daily trader level

Align trader metrics with Fear/Greed sentiment

Generate summary tables in the notebook

Save output charts and tables in the charts/ directory

📊 Methodology (Summary)

Trades are aggregated at a daily trader level

Key metrics computed include:

daily PnL

win rate

number of trades per day

average position size (leverage proxy)

long/short bias

Trader metrics are aligned with daily Fear / Greed sentiment

Insights are validated using tables and visualizations (boxplots and bar charts)

No future information is used, avoiding look-ahead bias

💡 Key Insights

Performance differs by sentiment
Traders achieve higher average daily PnL during Greed periods, but with higher volatility.

Trader behavior becomes more aggressive during Greed
Trade frequency and average position size increase during Greed days, indicating higher risk appetite.

Long bias increases without proportional improvement in win rate
Stronger long positioning during Greed does not translate into significantly better win rates, suggesting potential overconfidence.

All insights are supported by corresponding tables and charts included in the notebook and saved in the charts/ directory.

🎯 Strategy Recommendations

Sentiment-aware risk management
Reduce leverage and position size during Fear periods to limit drawdowns, while allowing normal or slightly higher exposure during Greed periods.

Selective activity scaling
Increase trade frequency during Greed regimes only for traders with historically consistent performance, rather than uniformly increasing activity.

📝 Notes

Output charts and tables are stored in the charts/ directory.

A concise written summary of methodology, insights, and strategies is available in insights.txt.

The analysis is fully reproducible using the steps above.