# Apple-stock-reactions-to-Quarterly-Earnings-reports
## Project Objective
This project analyzes the impact of Apple’s quarterly earnings reports on its stock price using historical market data from the Financial Modeling Prep (FMP) AP.
 The goal is to quantify and visualize market reactions using historical stock data.

---

## Data
- **Stock Prices:** Daily historical data from the [Financial Modeling Prep (FMP) API](https://financialmodelingprep.com/)  
- **Earnings Dates:** Verified from Apple’s official newsroom and FMP API  
- **Event Window:** ±3 trading days around each quarterly earnings date  

> **Note:** All data is publicly available and used here for educational purposes.

---

## Methodology

1. **Event Identification:** Last four Apple quarterly earnings dates:
   - Q4 2024: 2024-10-31  
   - Q1 2025: 2025-01-30  
   - Q2 2025: 2025-05-01  
   - Q3 2025: 2025-07-31  

2. **Event Window Creation:** ±3 trading days around each event.  

3. **Metrics (North Star Metrics):**
   - **Immediate Return (%):** Price change from t-1 to t+1  
   - **Extended Drift (%):** Price change from t-3 to t+3  
   - **Gap Return (%):** Overnight change between event day open and previous close  

4. **Visualizations:**  
   - Time-series plot with vertical markers for earnings events  
   - Bar chart comparing Immediate Return, Extended Drift, and Gap Return across quarters  

---

## Key Findings

| Quarter | Immediate Return % | Extended Drift % | Gap Return % |
|---------|------------------|-----------------|--------------|
| Q4 2024 | 1.39             | 2.84            | 0.84         |
| Q1 2025 | 2.58             | 4.23            | 0.40         |
| Q2 2025 | 3.00             | 5.60            | 1.05         |
| Q3 2025 | 3.91             | 5.59            | 0.86         |

**Observations:**  
- Positive immediate market reactions for most quarters  
- Extended drift suggests short-term momentum  
- Gap return captures overnight reactions, typically smaller than immediate return  

---

## Visualizations

### Time-Series Plot
Shows Apple stock closing price over time with vertical markers indicating quarterly earnings events.

### Bar Chart
Compares Immediate Return, Extended Drift, and Gap Return for all four quarters.

*Example charts are included in the `/plots` directory of the repository.*

---

## How to Run
1. Clone the repository:  
```bash
git clone https://github.com/yourusername/apple-earnings-analysis.git
