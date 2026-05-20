# Part 2: RFM Segmentation & Retention Strategy
## D2C Customer Churn Intelligence & Retention API — Capstone

---

## Overview

This repository contains Part 2 of the D2C Customer Churn Capstone project.

The objective is to build RFM-based customer segments and recommend targeted retention actions **before any ML model is deployed**. This gives the business an actionable framework based purely on behavioural data.

---

## Repository Structure

```
churn-part2-rfm/
│
├── rfm_segmentation.ipynb     ← Main segmentation notebook
├── segments.csv               ← Output: customer_id + segment_name + features
├── retention_strategy.md      ← Retention actions per segment + budget priority
├── manual_review_cases.md     ← 8 customers with contradictory signals
├── requirements.txt           ← Python dependencies
├── charts/                    ← All saved chart outputs
│   ├── chart1_segment_distribution.png
│   ├── chart2_rfm_scores_by_segment.png
│   ├── chart3_churn_rate_by_segment.png
│   ├── chart4_revenue_by_segment.png
│   ├── chart5_nonrfm_signals_by_segment.png
│   └── chart6_recency_vs_monetary.png
└── README.md
```

---

## Dataset

The dataset package is available here:  
[Google Drive Dataset Link](https://drive.google.com/drive/folders/1PmLapJI1VSDgvl_AxARNKwM1MCd3WFX0?usp=sharing)

Download and place all CSV files in a `data/` folder before running the notebook.

**Files required in `data/`:**
- `orders.csv`
- `customers.csv`
- `churn_labels.csv`
- `support_tickets.csv`
- `web_events_snapshot.csv`
- `intervention_history.csv`
- `rfm_modeling_snapshot.csv` ← Primary table used for RFM features

---

## Setup Instructions

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/churn-part2-rfm.git
cd churn-part2-rfm

# 2. Create and activate virtual environment
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # Mac/Linux

# 3. Install dependencies
pip install -r requirements.txt

# 4. Download dataset and place CSVs in data/ folder

# 5. Launch Jupyter and run the notebook
jupyter notebook rfm_segmentation.ipynb
```

---

## Segmentation Approach

### RFM Features
Built using `rfm_modeling_snapshot.csv` (pre-snapshot features, no leakage):

| Feature | Description |
|---|---|
| `recency_days` | Days since last purchase — lower is better |
| `frequency_180d` | Number of orders in last 180 days |
| `monetary_180d` | Total spend in last 180 days (INR) |

### Non-RFM Signals
Two additional signal categories combined with RFM:

| Signal | Source | Purpose |
|---|---|---|
| `return_rate_180d` | orders.csv | Dissatisfaction indicator |
| `avg_discount_pct_180d` | orders.csv | Price sensitivity |
| `ticket_count_90d` | support_tickets.csv | Support friction |
| `negative_ticket_rate_90d` | support_tickets.csv | Complaint quality |
| `sessions_30d` | web_events_snapshot.csv | App engagement |

---

## Segments & Results

| Segment | Count | % | Churn Rate | Avg Revenue |
|---|---|---|---|---|
| Dormant Customers | 875 | 36.5% | 66% | ₹544 |
| Discount-Sensitive | 502 | 20.9% | 54% | ₹654 |
| Champions | 388 | 16.2% | 10% | ₹2,432 |
| Loyal Customers | 374 | 15.6% | 25% | ₹1,601 |
| At-Risk Customers | 223 | 9.3% | 64% | ₹1,767 |
| High-Value but Unhappy | 38 | 1.6% | 16% | ₹2,363 |

---

## Campaign Budget Priority

1. **At-Risk Customers** — High revenue + high churn = best ROI
2. **High-Value but Unhappy** — Small group, high value, personal outreach
3. **Loyal Customers** — Potential to upgrade to Champions
4. **Discount-Sensitive** — Value-add offers, not discounts
5. **Dormant Customers** — One low-cost email only
6. **Champions** — Light touch, maintain relationship

---

## Key Files Explained

| File | Description |
|---|---|
| `rfm_segmentation.ipynb` | Full notebook: RFM scoring, segmentation logic, 6 charts, segment analysis |
| `segments.csv` | One row per customer with segment name and all key features |
| `retention_strategy.md` | Detailed strategy per segment with business rationale and budget prioritization |
| `manual_review_cases.md` | 8 edge cases with contradictory signals and individual reasoning |

---

## Notes

- `data/` folder excluded from version control via `.gitignore`
- All features use pre-snapshot data only (`order_date <= 2025-09-30`) to prevent leakage
- `rfm_modeling_snapshot.csv` is the primary feature source — all features are leakage-free per data dictionary
