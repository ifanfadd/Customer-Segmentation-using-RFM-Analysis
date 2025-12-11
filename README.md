# Customer-Segmentation-using-RFM-Analysis
A data-driven project that segments customers using Recency, Frequency, and Monetary metrics. Python (Colab) is used for data processing, RFM scoring, and exploratory analysis. An interactive Power BI dashboard visualizes customer groups, highlights behavior patterns, and supports better marketing and retention strategies.

---

## Table of Contents
- [Case Study](#-case-study)
- [Methodology: RFM](#-methodology-rfm)
- [Data Analysis & Visualization](#-data-analysis--visualization)
- [Customer Segmentation Results](#-customer-segmentation-results)
- [Strategic Recommendations](#-strategic-recommendations)

---

## Case Study
This analysis focuses on understanding and segmenting the customer base based on their transactional behavior (RFM).
1. **Evaluate the relationship** between Recency, Frequency, and Monetary value.
2. **Quantify the size** of each critical customer segment.
3. **Develop actionable insights** for retention, loyalty, and win-back campaigns.

---

## Methodology: RFM
RFM is a marketing technique used to quantitatively rank and group customers based on their behavior:

- **Recency (R):** Days since the last purchase (Lower is better).
- **Frequency (F):** Total number of purchases (Higher is better).
- **Monetary (M):** Total amount spent (Higher is better).

---

### 1. Recency vs. Monetary (R-M Plot)

<img width="593" height="460" alt="Image" src="https://github.com/user-attachments/assets/e9f19f0c-567f-4cad-88c8-d72320063556" />
 
There is a **strong inverse relationship** (negative correlation) between Recency and Monetary value.

* **High Value (Monetary $\uparrow$)** is concentrated among the **Most Recent Customers** (Recency $\approx 0-50$ days). The highest revenue earners are exclusively in this group.
* **Low Value (Monetary $\downarrow$)** dominates the segment of **Lapsed Customers** (Recency $\approx 200+$ days), where revenue contribution is minimal.
* **Insight:** Recency is the **most critical driver** of potential high revenue in this dataset.

### 2. Frequency vs. Monetary (F-M Plot)

<img width="593" height="460" alt="Image" src="https://github.com/user-attachments/assets/3427e5cb-84e8-4ff3-b40d-258e73fc6d13" />

There is **no clear strong correlation** between Frequency and Monetary value.

* **High Value (Monetary $\uparrow$)** is distributed across **all Frequency levels** (e.g., customers with 2 purchases vs. 10 purchases can generate the same high revenue).
* **Insight:** A customer's total value is determined by the size of their **individual transactions**, not just the quantity of transactions. High Frequency alone does not guarantee high revenue.

---

## Customer Segmentation Results
The RFM scores were used to segment the customer base into 11 distinct groups. The following table highlights the size of the most critical segments based on the counts provided:

| Rank | Customer Segment | Number of Customers | Implication & Strategy Focus |
| :--- | :--- | :--- | :--- |
| **1** | **Evasive Customer** | **596** | **Largest Group.** Low value, low engagement (low R, F, M). Strategy: Low-priority targeting; focus resources on higher-potential segments. |
| **2** | **Potential Customer** | **564** | **New/Recent, but not Frequent.** Strategy: Nurture them and encourage a quick second purchase through tailored recommendations. |
| **3** | **High Risk Customer** | **529** | **Lapsed but High Past Value.** Strategy: **Highest Priority Win-Back.** Implement aggressive, personalized offers immediately to prevent churn. |
| **4** | **Late Bloomer** | **526** | **Recently Active after a long lapse.** Strategy: Encourage maintenance of activity and reward their recent engagement. |
| **5** | **Lost Customer** | **503** | **Lapsed and Low Value.** Strategy: Low-effort win-back campaigns or minimal resource allocation due to low expected ROI. |
| **6** | **Loosing Customer** | **452** | **On the path to becoming "Lost" or "High Risk".** Strategy: Targeted promotions to stabilize their purchase behavior and halt the decline. |
| **7** | **Recent Customer** | **432** | **Bought recently, but F/M scores are not yet high.** Strategy: Focus on encouraging a rapid second purchase to boost Frequency. |
| **8** | **Almost Lost Customer** | **405** | **A high-risk group very close to being written off.** Strategy: High-touch, personalized outreach efforts. |
| **9** | **Very Loyal** | **357** | **Current Best Customers (High R, F, M).** Strategy: **Retention & Loyalty.** Offer exclusive rewards and VIP service to maximize Lifetime Value (LTV). |
| **10** | **Becoming Loyal** | **341** | **Showing good buying habits, moving toward the "Very Loyal" tier.** Strategy: Encourage further increases in purchase frequency. |
| **11** | **Platinum Customer** | **295** | **Most Elite, Highest Value.** Strategy: **Top Tier Retention.** High-touch, personalized service and early access to products/sales. |

### **Overall Segmentation Insight (Finalized)**

The total customer base is dominated by low-value and high-risk segments (the top 8 groups account for over 4,000 customers). Your most valuable and loyal customers—the **Very Loyal**, **Becoming Loyal**, and **Platinum Customer** segments (totaling 993 customers)—represent the smallest portion of the base, underscoring the critical need to focus resources on both **churn prevention** (High Risk) and **loyalty development** (Moving Potential/Recent customers into higher tiers).

## Strategic Recommendations
Based on the analysis, the following strategies are recommended:

### 1. Retention (Focus on High Risk & Loosing)
* **Goal:** Stop high-value customers from churning.
* **Action:** Immediately target the **High Risk Customer (529)** segment with high-value incentives (e.g., 20% off next purchase) to trigger a recent purchase and improve their Recency score.

### 2. Loyalty (Focus on Very Loyal & Platinum)
* **Goal:** Reward and maximize spending from top customers.
* **Action:** Implement a **VIP program** for the **Very Loyal (357)** and **Platinum ($\approx 300$)** segments, offering early access to sales or free premium shipping to maintain high Monetary and Frequency.

### 3. Growth (Focus on Potential & Recent)
* **Goal:** Move new customers into higher-value tiers.
* **Action:** Target **Potential Customer (564)** and **Recent Customer (432)** with personalized product recommendations based on their first purchase, aiming for a second transaction within 30 days to increase Frequency.

---

## Dashboard (Customer Segmentation Overview)

This bar chart visually confirms the distribution of the customer base, highlighting the large size of the low-value/high-risk segments compared to the loyal segments.

![Image](https://github.com/user-attachments/assets/1023d910-9722-4d21-80b3-0677cd759b86)


