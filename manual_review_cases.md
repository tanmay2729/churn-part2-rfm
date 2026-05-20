# Manual Review Cases
## D2C Customer Churn Intelligence — Part 2

These are 8 customers where the retention decision is **not straightforward** due to contradictory signals. Standard segment rules alone are insufficient — each requires individual reasoning.

---

### Case 1 — CUST00004
**Segment:** Dormant Customers  
**RFM:** R=2, F=2, M=4 | Score=8  
**Key stats:** Recency=131 days, Frequency=1, Monetary=₹1,604, Return Rate=0%, Tickets=0, Sessions=1, Churn=1

**Why it's complex:**  
This customer has a **high monetary score (M=4)** — spent ₹1,604 — but only placed 1 order and hasn't returned in 131 days. They are classified as Dormant but their single purchase was high-value. Standard dormant treatment (low investment) may be wrong here.

**Recommended action:**  
Treat as a lapsed high-value customer. Send a personalised win-back offer tied to their original purchase category. One high-quality outreach is worth the investment given their spend potential.

---

### Case 2 — CUST00042
**Segment:** High-Value but Unhappy  
**RFM:** R=2, F=5, M=5 | Score=12  
**Key stats:** Recency=87 days, Frequency=5, Monetary=₹4,306, Return Rate=0%, Tickets=2, Sessions=3, Churn=0

**Why it's complex:**  
Extremely high frequency (F=5) and monetary (M=5) — one of the best buyers. But recency has dropped to 87 days and they have 2 support tickets. Despite being labelled High-Value but Unhappy, they have NOT churned yet. The question is whether their silence (87 days) signals upcoming churn.

**Recommended action:**  
Immediate proactive outreach — acknowledge their tickets and offer priority resolution. Do not wait for them to churn. A personal call from customer success would be appropriate given their ₹4,306 spend.

---

### Case 3 — CUST00057
**Segment:** Dormant Customers  
**RFM:** R=2, F=2, M=4 | Score=8  
**Key stats:** Recency=136 days, Frequency=1, Monetary=₹1,713, Return Rate=0%, Tickets=0, Sessions=7, Churn=1

**Why it's complex:**  
Similar to CUST00004 — high monetary but low frequency. However this customer has **7 app sessions** despite not buying for 136 days. They are browsing but not converting — a classic "window shopper" pattern. They have already churned (churn=1).

**Recommended action:**  
Target with a conversion-focused campaign — they are clearly still interested (7 sessions) but something is stopping them from buying. A targeted discount on their browsed category may convert them back.

---

### Case 4 — CUST00178
**Segment:** High-Value but Unhappy  
**RFM:** R=5, F=4, M=4 | Score=13  
**Key stats:** Recency=5 days, Frequency=2, Monetary=₹1,584, Return Rate=100%, Tickets=2, Sessions=10, Churn=0

**Why it's complex:**  
This customer has a **100% return rate** — every order has been returned — yet they keep coming back (recency=5 days, sessions=10). They are highly engaged but clearly dissatisfied with product quality or fit. Standard churn risk models would miss this.

**Recommended action:**  
This is a product-fit issue, not a churn issue. Recommend a personalised consultation or skin/product quiz to help them find the right product. Do not offer discounts — they are already buying. Fix the return reason first.

---

### Case 5 — CUST00263
**Segment:** Champions  
**RFM:** R=4, F=5, M=4 | Score=13  
**Key stats:** Recency=25 days, Frequency=3, Monetary=₹1,618, Return Rate=67%, Tickets=2, Sessions=15, Churn=0

**Why it's complex:**  
Classified as a Champion (high RFM) but has a **67% return rate** and 2 tickets. Champions are typically treated with light-touch retention, but this customer's high return rate is a hidden risk. They are highly engaged (15 sessions) but returning 2 out of 3 orders.

**Recommended action:**  
Do not treat as a standard Champion. Proactively reach out to understand return reasons. May be a sizing/product matching issue. Resolve before return rate increases further — this customer is at risk of souring despite high engagement.

---

### Case 6 — CUST00438
**Segment:** High-Value but Unhappy  
**RFM:** R=3, F=5, M=5 | Score=13  
**Key stats:** Recency=64 days, Frequency=3, Monetary=₹2,466, Return Rate=100%, Tickets=2, Sessions=6, Churn=1

**Why it's complex:**  
Very high monetary (₹2,466) and frequency (F=5) but **100% return rate** and has already churned. Despite spending a lot, they returned everything. This is an extreme dissatisfaction case — every purchase was returned before churning.

**Recommended action:**  
Standard win-back campaigns will not work here. Requires a root cause investigation — what went wrong? A direct personal outreach with a genuine apology and product replacement offer may be the only chance of recovery. Flag for senior customer success review.

---

### Case 7 — CUST00025
**Segment:** Discount-Sensitive  
**RFM:** R=1, F=2, M=2 | Score=5  
**Key stats:** Recency=165 days, Frequency=1, Monetary=₹518, Return Rate=0%, Tickets=0, Sessions=11, Churn=1

**Why it's complex:**  
Low RFM score but **11 app sessions** — very high browsing activity despite not buying for 165 days. Classified as Discount-Sensitive but their engagement suggests they may respond to a non-discount trigger. They have churned (churn=1).

**Recommended action:**  
Don't write off with a standard dormant treatment. Their 11 sessions show clear interest. Test a personalised "new arrival" or "trending product" email rather than a discount — they may be waiting for the right product, not the right price.

---

### Case 8 — CUST00066
**Segment:** Dormant Customers  
**RFM:** R=1, F=1, M=1 | Score=3  
**Key stats:** Recency=320 days, Frequency=0, Monetary=₹0, Return Rate=0%, Tickets=0, Sessions=11, Churn=1

**Why it's complex:**  
The lowest possible RFM score (3) — no orders, no revenue, no tickets, 320 days since last visit. Should be the easiest dormant case. But they have **11 app sessions** — meaning they are still actively browsing the app despite never converting and having churned.

**Recommended action:**  
This is a pure conversion problem, not a retention problem. They were never truly a customer — they browsed but never bought. Do not spend retention budget here. Instead flag for the acquisition/conversion team to understand what barrier exists. A first-purchase incentive may convert them.

---

## Summary Table

| Customer ID | Segment | Core Contradiction | Churn | Recommended Priority |
|---|---|---|---|---|
| CUST00004 | Dormant | High M but only 1 order, 131 days silent | Yes | Medium — worth one personalised outreach |
| CUST00042 | High-Value Unhappy | Highest F+M but recency dropping | No | High — proactive call before churn |
| CUST00057 | Dormant | High M, 7 sessions but not buying | Yes | Medium — conversion campaign |
| CUST00178 | High-Value Unhappy | 100% return rate but keeps coming back | No | High — product-fit intervention |
| CUST00263 | Champions | Champion label but 67% return rate | No | High — hidden risk in top segment |
| CUST00438 | High-Value Unhappy | ₹2,466 spend but 100% returned + churned | Yes | High — senior review needed |
| CUST00025 | Discount-Sensitive | Low RFM but 11 sessions — interested | Yes | Low-Medium — new arrival campaign |
| CUST00066 | Dormant | Zero revenue but 11 sessions | Yes | Low — pass to acquisition team |
