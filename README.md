# 🏦 Bank Telemarketing EDA — Term Deposit Subscription Analysis

## 📌 Project Overview

**Bank of Corporate** conducted a telemarketing campaign for **Term Deposits** targeting existing customers. This project performs a full Exploratory Data Analysis (EDA) to identify the right customer profiles to target and uncover the key drivers behind successful conversions.

This was completed as part of the **PwC Academy Business Analytics & Consulting Program (UpGrad)**.

---

## 🎯 Business Objective

> *"Identify the target customers and the driving factors behind a successful customer conversion for future telemarketing campaigns."*

- Who is most likely to subscribe to a term deposit?
- What call patterns and customer attributes drive conversions?
- Which customer segments should be prioritized?

---

## 🗂️ Dataset

| Detail | Info |
|---|---|
| Domain | BFSI — Retail Banking |
| Product | Term Deposit Subscription |
| Overall Conversion Rate | **11.54%** |
| Features | 18 columns (customer attributes + campaign attributes) |

**Key Columns:**

| Column | Description |
|---|---|
| Age, Job, Marital Status, Education | Customer profile attributes |
| Loan Default, Housing Loan, Personal Loan | Credit behaviour |
| Cash Balance | Account health indicator |
| Contact, Call Duration | Campaign outreach details |
| pdays, previous, poutcome | Previous campaign history |
| Subscription | Target variable (1 = subscribed, 0 = not subscribed) |

---

## 🛠️ Tools & Techniques Used

- **Microsoft Excel** — Data Cleaning, EDA, Charts, Pivot Analysis
- **PowerPoint** — Insight communication & business recommendations
- **Univariate Analysis** — Distribution of each variable
- **Bivariate Analysis** — Subscription rate across customer segments
- **Segmented Analysis** — Marital status × Education cross-tab

---

## 🧹 Data Cleaning Steps

1. Removed duplicate rows
2. Removed rows with blank values (Loan Default, Subscription, poutcome)
3. Converted negative Age values to positive
4. Standardized Job field (`admin.` → `admin`)
5. Encoded binary fields: `yes` → 1, `no` → 0 (Loan Default, Housing Loan, Personal Loan, Subscription)
6. Converted Date from text format to Excel Date format
7. Extracted `Day` and `Month` columns from the Date field
8. Converted Call Duration from Hrs/Mins/Sec format to seconds
9. Removed outliers in the `Previous` column

---

## 📊 Key Analysis & Findings

### Univariate Analysis
- **Age:** Majority of customers fall in the 23–60 working-age range; steep decline after 60
- **Job:** Blue-collar and Management are the dominant customer segments
- **Loan Default:** Only 1.80% of customers have defaulted — low credit risk pool
- **Month:** 30.51% of all calls made in **May** — highest outreach month
- **Day:** Bank preferentially contacts customers on **weekends** (working population behaviour)
- **Call Duration:** Most calls last between **1–3 minutes**; median ≈ 180 seconds

### Bivariate Analysis (vs Subscription)
| Factor | Key Finding |
|---|---|
| Education | **Doctorate holders** convert better than Masters/Bachelors |
| Marital Status | **Unmarried customers** show higher conversion rates |
| Call Duration | Subscribed customers have **significantly longer call durations** |
| poutcome | Customers who **previously subscribed to other products** convert better |
| Month | **March** has the highest conversion rate — end of financial year effect |
| Previous Calls | Conversion drops sharply after **8 prior contacts** — stop re-contacting beyond this |
| pdays | Customers respond better when contacted **quarterly or semi-annually** |

---

## 💡 Business Recommendations

| # | Recommendation |
|---|---|
| 1 | **Target Doctorate-educated unmarried customers first** — highest conversion probability |
| 2 | **Prioritize March campaigns** — end of financial year drives long-term investment intent |
| 3 | **Do not contact customers with 8+ prior calls** — diminishing returns confirmed |
| 4 | **Focus on customers with prior product subscriptions** — warm leads convert better |
| 5 | **Train agents for longer calls** — call duration is strongly linked to conversion |
| 6 | **Space out outreach quarterly/semi-annually** — over-contacting hurts conversion |

---

## 📁 Repository Structure

```
bank-telemarketing-eda/
│
├── Data-Dictionary.xlsx          # Column definitions for all 18 fields
├── Data-set-Stub-file.xlsx       # Original raw dataset
├── Dataset-Cleaned.xlsx          # Cleaned dataset used for analysis
├── Solution-PPT-BA-1-.pptx       # 20-slide EDA presentation with charts & recommendations
└── README.md                     # Project documentation (this file)
```

---

## ▶️ How to Explore

1. Start with `Data-Dictionary.xlsx` to understand each column
2. Compare `Data-set-Stub-file.xlsx` vs `Dataset-Cleaned.xlsx` to see data cleaning steps
3. Open `Solution-PPT-BA-1-.pptx` for the full visual analysis — 20 slides covering univariate, bivariate, and segmented analysis with business recommendations

---

## 🧠 Skills Demonstrated

- End-to-end data cleaning (outlier removal, encoding, format conversion)
- Univariate and bivariate EDA with business context
- Customer segmentation analysis (marital status × education cross-tab)
- Insight communication through structured PowerPoint storytelling
- BFSI domain knowledge — telemarketing campaign strategy

---

## 👤 Author

**Jebaz Jeeva M**  
PGDM — Business Analytics & Marketing | Rajalakshmi School of Business  
[LinkedIn](https://www.linkedin.com/in/jebazjeeva/) | [GitHub](https://github.com/JebazJeeva)
