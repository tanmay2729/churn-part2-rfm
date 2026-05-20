# Retention Strategy Report
## D2C Customer Churn Intelligence — Part 2

**Snapshot Date:** 2025-09-30  
**Total Customers Segmented:** 2,400  
**Segmentation Method:** RFM Scoring + Non-RFM Signals (return rate, support tickets, app sessions, discount usage)

---

## Segment Overview

| Segment | Count | % | Churn Rate | Avg Revenue | Avg Recency | Avg Sessions |
|---|---|---|---|---|---|---|
| Dormant Customers | 875 | 36.5% | 66% | ₹544.67 | 135.63 days | 4.40 |
| Discount-Sensitive | 502 | 20.9% | 54% | ₹654.06 | 72.92 days | 5.35 |
| Champions | 388 | 16.2% | 10% | ₹2,432.53 | 20.98 days | 7.45 |
| Loyal Customers | 374 | 15.6% | 25% | ₹1,601.13 | 50.87 days | 6.15 |
| At-Risk Customers | 223 | 9.3% | 64% | ₹1,767.04 | 117.86 days | 4.83 |
| High-Value but Unhappy | 38 | 1.6% | 16% | ₹2,363.40 | 25.61 days | 7.74 |

---

## Segment Deep Dives & Retention Actions

---

### 1. Champions (388 customers — 10% churn rate)

**Who they are:**  
Most recent, most frequent, highest spending customers. Average recency of just 21 days, avg revenue ₹2,432 in 180 days, avg 7.45 sessions/month. Churn rate is only 10% — these are your best customers.

**Non-RFM signals:**  
Low support tickets (0.39 avg), low return rate (7%), high app engagement.

**Retention Action:**  
- Do NOT over-discount — they buy without incentive
- Offer early access to new product launches
- Enroll in loyalty/VIP programme if not already enrolled
- Send personalised thank-you communications

**Expected Business Value:**  
Protecting this segment prevents the highest revenue loss. Each churned Champion costs ~₹2,432 in revenue per 180 days.

---

### 2. Loyal Customers (374 customers — 25% churn rate)

**Who they are:**  
Regular buyers with decent recency (51 days avg) and good revenue (₹1,601 avg). Churn rate of 25% means 1 in 4 is at risk — worth investing in to move them toward Champions.

**Non-RFM signals:**  
Low support tickets (0.31 avg), low return rate (5%), moderate app engagement (6.15 sessions).

**Retention Action:**  
- Offer loyalty rewards and points programmes
- Send personalised product recommendations based on purchase history
- Target with bundle offers to increase order value
- Re-engage those with recency > 45 days with a "We miss you" campaign

**Expected Business Value:**  
Moving even 20% of Loyal Customers to Champions adds ~₹831 per customer in additional revenue (difference between ₹1,601 and ₹2,432).

---

### 3. At-Risk Customers (223 customers — 64% churn rate)

**Who they are:**  
Previously good customers (avg frequency 2.38, avg revenue ₹1,767) who have gone quiet — avg recency of 118 days. Second highest churn rate at 64%. These are lapsed high-value customers.

**Non-RFM signals:**  
Low sessions (4.83), low support tickets (0.06), low return rate (7%). Their silence is the warning sign.

**Retention Action:**  
- **Priority: HIGH** — act before they churn completely
- Send win-back campaign with a time-limited offer (not blanket discount)
- Personalise outreach based on their last purchased category
- Trigger email/push for customers with recency > 90 days

**Expected Business Value:**  
Winning back even 30% of At-Risk customers at their historical revenue (₹1,767) = ₹118,190 recovered revenue.

---

### 4. Discount-Sensitive Customers (502 customers — 54% churn rate)

**Who they are:**  
Customers who primarily buy when discounts are high (avg discount 39%). Low revenue (₹654 avg), moderate recency (73 days). High churn rate of 54% — they leave when discounts stop.

**Non-RFM signals:**  
Low tickets (0.19 avg), low return rate (6%), moderate sessions (5.35).

**Retention Action:**  
- Avoid training them further on discounts — breaks margin
- Instead offer value-adds: free samples, bundle deals, loyalty points
- Test reducing discount depth gradually to improve margin
- Identify subset who show increasing engagement — potential to convert to Loyal

**Expected Business Value:**  
Reducing discount dependency by 10% across this segment saves significant margin without necessarily losing customers.

---

### 5. Dormant Customers (875 customers — 66% churn rate)

**Who they are:**  
Largest segment at 36.5% of customers. Lowest revenue (₹544 avg), highest recency (136 days avg), lowest sessions (4.40). Churn rate of 66% — most are already effectively churned.

**Non-RFM signals:**  
Very low tickets (0.11), low return rate (5%), lowest engagement overall.

**Retention Action:**  
- **Do NOT invest heavy budget here** — ROI is lowest
- Send one low-cost win-back email campaign
- If no response in 30 days, suppress from future campaigns
- Focus budget on At-Risk and Loyal segments instead
- Small subset with high monetary history (M>=3) worth a personal outreach

**Expected Business Value:**  
Even a 5% win-back rate across 875 customers = 43 customers recovered at ₹544 avg = ₹23,392 revenue.

---

### 6. High-Value but Unhappy (38 customers — 16% churn rate)

**Who they are:**  
Small but critical segment. High revenue (₹2,363 avg), recent purchasers (26 days avg), but high support ticket volume (2.08 avg tickets) and high return rate (35%). Despite complaints, only 16% have churned — they still value the products but are frustrated.

**Non-RFM signals:**  
Highest return rate (35%), highest ticket count (2.08), but still active (7.74 sessions).

**Retention Action:**  
- **Escalate immediately to customer success team**
- Proactively resolve all open tickets before next purchase
- Assign dedicated account manager or priority support
- Do NOT send generic discount — personalised apology + service guarantee works better

**Expected Business Value:**  
Each customer is worth ₹2,363 per 180 days. Retaining all 38 = ₹89,794 protected revenue. High ROI on personal outreach investment.

---

## Campaign Budget Prioritisation

With a limited campaign budget, prioritise segments in this order:

| Priority | Segment | Reason |
|---|---|---|
| 1st | At-Risk Customers | High revenue (₹1,767) + high churn risk (64%) = highest ROI on win-back |
| 2nd | High-Value but Unhappy | Small group, high value (₹2,363), personal outreach is low cost |
| 3rd | Loyal Customers | Moderate churn (25%), high potential to upgrade to Champions |
| 4th | Discount-Sensitive | Large group but low revenue — focus on value-add not discounts |
| 5th | Dormant Customers | Lowest ROI — one low-cost email only |
| 6th | Champions | Lowest churn risk — maintain relationship, no heavy spend needed |

**Key principle:** Never spend the same amount per customer across all segments. At-Risk and High-Value but Unhappy deserve 3-5x more spend per customer than Dormant.

---

## Non-RFM Signals Used

| Signal | Source | Why Included |
|---|---|---|
| `return_rate_180d` | orders.csv | High returns = dissatisfaction = churn risk |
| `ticket_count_90d` | support_tickets.csv | Support volume indicates friction |
| `negative_ticket_rate_90d` | support_tickets.csv | Quality of complaints, not just quantity |
| `sessions_30d` | web_events_snapshot.csv | App engagement = interest level |
| `avg_discount_pct_180d` | orders.csv | Discount dependency = price sensitivity |
