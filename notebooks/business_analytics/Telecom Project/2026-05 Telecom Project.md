# Revenue Analysis Across Mobile Plans for a Telecom Operator

## 📊 Project Overview

**Business Context**: A federal mobile network operator seeks to optimize advertising budget allocation by analyzing customer usage patterns and determining which tariff plan generates higher revenue.

**Dataset**: Sample of 500 users with demographics, subscription details, and complete 2018 usage data (calls, messages, internet sessions).

**Key Business Question**: Which tariff plan (Smart vs Ultra) is more profitable for the operator?


## 📁 Data Sources

| Dataset | Records | Description |
|---------|---------|-------------|
| `users.csv` | 500 | User demographics, subscription dates, tariff plans |
| `calls.csv` | ~20k | Call records with duration and dates |
| `messages.csv` | ~80k | SMS/text message records |
| `internet.csv` | ~80k | Internet usage sessions with data consumption |
| `tariffs.csv` | 2 | Tariff plan details and pricing structure |

## 📝 Notes & Assumptions

**Business Rules Applied:**
- Call duration rounded up to nearest minute (company policy)
- Data overage charged per full GB (partial GB rounded up)
- Monthly billing cycles used for revenue aggregation

**Data Quality Considerations:**
- Missing usage data treated as zero usage (non-active users)
- Churn date NULL indicates active subscription through data period
- Age data aggregated into 5-year bins for privacy

**Analytical Limitations:**
- Cost data not available (network costs, customer acquisition costs)
- External factors not considered (competition, market conditions)
- Sample size limited to 500 users 