# Kraken Product Analytics Dashboard (Growth Case Study)

This project is an end-to-end **Product & Growth Analytics case study** inspired by the work expected of a **Data Analyst, Product (Growth)** at Kraken.

It demonstrates how data can be transformed into actionable insights through scalable pipelines, KPI design, experimentation, retention analysis, and executive-ready dashboards.

---

## Project Overview

The goal of this project is to simulate how a Product Data Analyst supports growth decision-making at a crypto platform by answering questions such as:

- How strong is early user activation?
- Which acquisition channels drive the highest-quality users?
- Where are the largest funnel drop-offs?
- What is user retention over time?
- Are experiments statistically meaningful?
- How much traffic is required to detect small conversion lifts?

---

## Key Analytics Delivered

### Activation Funnel (7-Day)

- **Deposit Conversion (7D):** ~30.7%  
- **Trade Conversion (7D):** ~21.4%

A meaningful segment of users deposit but do not trade within their first week, highlighting an activation opportunity.

---

### Acquisition Channel Performance

Channel-level segmentation reveals:

- Affiliate and Paid Social drive strong early activation  
- Organic drives the largest total revenue due to scale  
- Influencer traffic shows fewer but higher-value traders (high ARPT)

---

### Monetization Metrics

Revenue analysis includes:

- Trading fee contribution by channel  
- **ARPU (Average Revenue Per User)**  
- **ARPT (Average Revenue Per Trader)**  

These metrics support budget allocation decisions beyond conversion rates alone.

---

### Retention & Cohort Analysis

Retention modeling includes:

- Weekly signup cohorts  
- D1 / D7 / D30 retention tracking  
- Retention curve decay over time  

This provides visibility into long-term engagement beyond activation.

---

### Experimentation & A/B Testing

A simulated onboarding experiment evaluates 7-day deposit conversion:

- Control vs Treatment conversion comparison  
- Z-test for statistical significance  
- Sample size and Minimum Detectable Effect (MDE) planning  

Key takeaway: small lifts require substantial traffic and long experiment duration.

---

## Dashboard Layer (Streamlit)

A multi-page Streamlit dashboard was built to provide leadership-ready reporting:

- Daily KPI monitoring  
- Funnel performance  
- Channel conversion + revenue breakdown  
- Retention cohorts  
- Experiment evaluation + power planning  

---

## Repository Structure

```bash
kraken-product-analytics/
│
├── app/                    # Streamlit dashboard application
│   ├── Home.py
│   └── pages/
│       ├── Funnel.py
│       ├── Channels.py
│       ├── Retention.py
│       ├── Experiments.py
│       └── Experiment_Planning.py
│
├── notebooks/              # Analytics workflow scripts
│
├── scripts/                # Dataset generator
│   └── generate_dataset.py
│
├── data/                   # Synthetic raw event-level data
│
├── outputs/                # Gold KPI tables + insight summaries
│
├── requirements.txt
└── runtime.txt
