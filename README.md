# ACC102-Track2
for acc102 mini assignment
# Historical Volatility & Risk Analysis Tool

## 1. Problem & User
This project addresses the need for **automated risk assessment** in financial trading. It is designed for **retail investors and analysts** who need to quickly identify historical extreme market movements and calculate asset volatility without using expensive financial terminals.

## 2. Data
- **Source:** [Kaggle]
- **Access Date:** April 22, 2026
- **Key Fields:**
    - `Date`: The trading date (set as index).
    - `Daily Return`: Percentage change in price from the previous day.

## 3. Methods
The analysis is performed using **Python (Pandas & Matplotlib)** through the following steps:
1. **Data Ingestion:** Loading the dataset into a Pandas DataFrame.
2. **Preprocessing:** Converting the 'Date' column to a DateTime index to enable time-series slicing.
3. **Statistical Calculation:** Computing the standard deviation of daily returns to determine volatility.
4. **Extrema Identification:** Using `idxmax()` and `idxmin()` to locate the specific dates of maximum gain and loss.

## 4. Key Findings
Based on the historical data analysis, the following insights were generated:
- **Max Single-Day Gain:** **24.40%**, occurring on **2013-05-09**.
- **Max Single-Day Loss:** **-21.06%**, occurring on **2020-09-08**.
- **Average Daily Volatility:** The asset exhibits a standard deviation of **3.56%**, indicating a high-risk profile compared to broader market indices.

## 5. How to run
1. Ensure you have Python 3 installed.
2. Install necessary libraries: `pip install pandas matplotlib`
3. Open `ACC102(1).ipynb` in Jupyter Lab or Notebook.
4. Run all cells to generate the summary statistics and charts.

## 6. Product link / Demo
- **Demo Video:** https://b23.tv/Qp9z4hG
- **Notebook:** See 'ACC102(1).ipynb` for the full code implementation.

## 7. Limitations & next steps
- **Limitations:** The current model assumes historical volatility is a perfect predictor of future risk, which may not always hold true during "black swan" events. The dataset is limited to [2010-2022].
- **Next Steps:**
    - Implement a rolling volatility window (e.g., 30-day moving volatility) to visualize risk changes over time.
    - Integrate real-time data API for live monitoring.
