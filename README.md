Telco Customer Churn Analysis (Task 2)

 Project Overview
An executive dashboard and churn analysis built in Microsoft Excel using the Kaggle Telco Customer Churn dataset (`7,043` total customer records).
 Key Findings & Executive KPIs
* **Total Customers:** 7,043
* **Churned Customers:** 1,869
* **Overall Churn Rate:** 27%
* **Monthly Revenue Lost:** $139,130.85

 Methodology & Dashboard Steps Performed
1. **Dataset Import & Validation:** Loaded the cleaned Telco Customer Churn dataset into Excel for dashboard aggregation.
2. **Executive KPI Layout:** Structured top-level summary cards in row 2 of the `Churn Analysis` tab with clean headers in row 1.
3. **Total Customer Count:** Calculated active records dynamically using `=COUNTA('Telco-Customer-Churn'!$A$2:$A$7044)`.
4. **Churn Count Aggregation:** Quantified churned customers using `=COUNTIF('Telco-Customer-Churn'!$U$2:$U$7044, "Yes")`.
5. **Overall Churn Rate:** Computed churn percentage using `=B2/A2` formatted as `27%`.
6. **Monthly Revenue Loss:** Aggregated total monthly revenue lost from churned users using `=SUMIF('Telco-Customer-Churn'!$U$2:$U$7044, "Yes", 'Telco-Customer-Churn'!$S$2:$S$7044)`.
7. **Formula Integrity:** Locked absolute cell ranges with `$` references to prevent formula drift across rows.
8. **Pivot Table 1 (Contract & Billing Averages):** Analyzed customer count and average `MonthlyCharges` broken down by `Contract` type and `Churn` status.
9. **Pivot Table 2 (Internet Service & Tenure Averages):** Tracked average customer lifespan (`tenure`) and average monthly bills across `InternetService` categories (DSL, Fiber optic, No).
10. **Pivot Table 3:** Examined customer distribution and average monthly charges across `PaymentMethod` types to isolate high-risk billing patterns.
