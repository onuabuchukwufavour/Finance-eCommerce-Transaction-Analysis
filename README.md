# Finance-eCommerce-Transaction-Analysis
# Project: Finance & eCommerce Transaction Analysis
**Prepared by:** Onuabuchukwu Favour Chimdindu

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Objectives](#objectives)
3. [Dataset Context](#dataset-context)
4. [Technologies Used](#technologies-used)
5. [Key Questions](#key-questions)
6. [Key Metrics](#key-metrics)
7. [Visualizations](#visualizations)
8. [Insights](#insights)
9. [Conclusion](#conclusion)
10. [Recommendations](#recommendations)

---

## Project Overview
The organization maintains a dataset of **6,056 financial transactions** with detailed information on accounts, merchants, locations, and fraud flags.  
The purpose of this project is to build a reliable system that analyzes transactions for operational insights and identifies potentially fraudulent activity.

---

## Objectives

- **Identify the most profitable merchants and categories**  
  Measure revenue contribution to understand top-earning areas.

- **Determine the most popular categories by transaction volume**  
  Show which categories receive the highest customer interactions.

- **Analyze merchant performance trends over time**  
  Track monthly revenue patterns to observe growth, decline, or seasonality.

- **Understand merchant–category relationships**  
  Use heatmaps to find which merchants dominate or diversify categories.

- **Compare revenue vs. transaction volume**  
  Identify high-revenue/low-volume vs. high-volume/low-revenue categories.

- **Provide insights for business decision-making**  
  Support decisions on onboarding, promotions, and resource allocation.

---

## Dataset Context
The dataset contains eCommerce transaction fields including:

- TransactionID  
- Date  
- AccountID, AccountName  
- TransactionType  
- Amount, Currency, ExchangeRate, Balance  
- Merchant, MerchantPhone  
- Category  
- IsFraud  

---

## Technologies Used

| Category              | Tools                        |
|-----------------------|------------------------------|
| Programming           | Python                       |
| Data Cleaning         | Pandas, NumPy                |
| Visualization         | Matplotlib, Seaborn          |
| Time/Date Handling    | datetime, Pandas datetime    |
| File Management       | OS module, CSV files         |
| Development Environment | Jupyter Notebook           |

---

## Key Questions

1. Identify top merchants by revenue and transaction count  
2. Analyze category popularity vs profitability  
3. Detect merchant-category trends and cross-selling opportunities  
4. Track monthly revenue trends  
5. Assess fraud patterns across merchants and categories  

---

## Key Metrics

- Total Revenue  
- Total Number of Transactions  
- Revenue per Category  
- Transaction Count per Merchant  
- Monthly Revenue Trend  
- Merchant–Category Interaction Matrix (Heatmap Data)

---

## Visualizations

### Bar Charts
- Top categories by **transaction volume**  
- Top categories by **revenue**  
- Category distribution (counts)

### Merchant × Category Heatmap
Shows transaction counts for each merchant across categories.

### Scatter Plot
Revenue vs. transaction volume per category.

### Line Plot
Monthly revenue trends for top merchants.

---

## Insights

### Fraud Analysis
- Converted `IsFraud` to `IsFraudFlag` (1 = Fraud, 0 = Legit) for quant analysis.  
- Merchant-level aggregation reveals which merchants have higher fraud tendencies.

### Transaction Patterns
- High volumes cluster around key merchants/categories (e.g., electronics, subscriptions).  
- Average transaction amounts vary widely (e.g., electronics > groceries).

### Account Behavior
- Some accounts consistently perform high-value transactions — useful for anomaly monitoring.

### Currency & Exchange Rate Impact
- Multi-currency transactions distort totals without conversion.  
- Standardization to a base currency improves accuracy.

---

## Conclusion
The analysis provides a deep understanding of merchant and category performance.  

- Clear differences in **category popularity** (volume) vs **profitability** (revenue).  
- Heatmaps reveal strong merchant–category relationships and dominance patterns.  
- Monthly revenue trends expose seasonal behavior and merchant performance shifts.  
- Revenue-to-volume relationships highlight both high-value and high-demand segments.  

**Business Implications:**
- Identify top merchants  
- Optimize low-performing categories  
- Plan targeted promotions  
- Improve resource allocation  
- Enhance fraud monitoring  

With expanded data (customer or product-level), the analysis can grow into segmentation, forecasting, and advanced fraud detection.

---

## Recommendations

### Fraud Prevention
- Monitor merchants and categories with high fraud rates.  
- Use `IsFraudFlag` for quick anomaly detection.

### Merchant & Category Monitoring
- Track revenue trends for top-selling merchants.  
- Investigate high-risk merchants to minimize losses.

### Account Review
- Flag accounts with unusually high or inconsistent transaction patterns.

### Currency Handling
- Standardize all amounts to a base currency.  
- Pay attention to exchange-rate-sensitive currencies.

### Data Quality
- Ensure merchant, transaction type, and fraud columns are complete and consistent.  
- Use dashboards for continuous trend and fraud monitoring.
