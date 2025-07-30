📊 Trading Behavior vs Market Sentiment Analysis

This project investigates the correlation between trader behavior (profitability, leverage, volume) and market sentiment using the Fear & Greed Index. It aims to identify how emotion-driven markets affect trading performance and provide strategic insights to optimize trading decisions.


---

🧠 Project Objective

Explore the relationship between trader performance and market sentiment

Uncover behavioral patterns under different emotional market states

Identify signals and trends to guide smarter trading strategies



---

📁 Datasets Used

historical_data.csv – Contains individual trader metrics: profit, trade count, volume, leverage, date

fear_greed_index.csv – Contains daily Fear & Greed Index values (0–100)



---

🔧 Setup Instructions

✅ Run in Google Colab (Recommended)

1. Open Google Colab


2. Upload the files:

historical_data.csv

fear_greed_index.csv



3. Open or copy the notebook code from: Trading_vs_Sentiment_Analysis_Project.ipynb


4. Run all cells step-by-step



💻 Run Locally

pip install pandas matplotlib seaborn plotly scikit-learn fpdf
jupyter notebook Trading_vs_Sentiment_Analysis_Project.ipynb


---

📊 Data Science Workflow

1. Data Loading & Inspection

Loaded both CSVs using pandas

Inspected columns, datatypes, null values, and descriptive statistics


2. Data Cleaning

Handled missing/null values

Converted and formatted date columns

Merged both datasets using the date as key


3. Sentiment Labeling

Transformed numerical sentiment into categories:

0–25 → Extreme Fear

26–45 → Fear

46–55 → Neutral

56–75 → Greed

76–100 → Extreme Greed


4. Exploratory Data Analysis (EDA)

Visual analyses to explore behavioral patterns across sentiment levels:

Profit vs Sentiment (Line Chart)

Average Leverage by Sentiment (Bar Chart)

Volume by Sentiment (Box Plot)

Sentiment Transitions vs Profitability (Heatmap)


5. Key Insights Extraction

Derived insights into:

How sentiment shifts affect behavior

Risky behavior spikes

Emotional decision-making footprints



---

📌 Key Insights

Profitability and Greed: Profitability increases under greed sentiment but often with increased volatility and inconsistent gains.

Risk and Leverage: Leverage peaks in Greed phases—suggesting risk-taking due to overconfidence.

Volume Surges: Significant trade volume increases during sentiment transitions (e.g., Fear ➝ Neutral or Greed ➝ Fear).

Lag Effect: Sentiment has a delayed effect—today’s sentiment correlates with tomorrow’s risk level.

Cluster Behavior: Traders fall into clusters based on emotional response, which can be identified using KMeans (optional step).



---

✅ Summary

This analysis reveals a strong interconnection between market sentiment and trading behavior.
Understanding how fear or greed shapes leverage, volume, and profitability allows for better:

Risk management

Emotion-aware strategy design

Timing of market entries/exits


By identifying these emotional patterns, traders and analysts can make informed, data-driven decisions.


---

🧾 Conclusion

Integrating sentiment analysis with trader behavior shows that:

High greed often leads to overleveraging and inconsistent gains

Fear phases, while conservative, offer stable behavior patterns

Sentiment transitions can be used as early signals for strategy pivots


This project bridges data science and behavioral finance to promote emotion-resilient, intelligent trading.


---

📂 Project Structure

├── historical_data.csv
├── fear_greed_index.csv
├── Trading_vs_Sentiment_Analysis_Project.ipynb
├── visuals/
│   ├── sentiment_vs_profit.png
│   ├── leverage_by_sentiment.png
│   └── volume_sentiment_boxplot.png
├── final_insights_report.pdf
├── README.md


---

🧑‍💻 Author

Muthuraj
Data Analyst | AI Digital Marketer | Portfolio Builder


---

📜 License

Open for learning, portfolio and academic use only.
