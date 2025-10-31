---
layout: single
title: Ninjacart
period: 2019-2021
---

# Ninjacart (2019-2021)
**Role:** Data Scientist

## Logistics Control Tower KPIs & Dashboard

Analyzed end-to-end control tower operations to establish key performance indicators for daily logistics management.

**Key Metrics Defined:**
- Transport Performance: on-time delivery, shipment delay rate
- Fleet Utilization: truck utilization
- Cost/Efficiency: cost per trolley

**Implementation:**
- Developed Google Looker Studio dashboard integrated with Google App Scripts
- Used by leadership for key decision making across logistics operations

**Tech Stack:** Google Looker Studio, Google App Scripts

---

## Supply Chain Model Change (DC to Micro-DC)

Analyzed Ninjacart's supply chain transformation from 1-2 large distribution centers on city outskirts to 15-20 smaller micro-DCs (dark stores) within cities.

**What I Did:**
- Determined optimal number and location of micro-DCs
- Analyzed capacities and order volumes
- Built optimization models for network design

**Impact:**
- Operational efficiency increased by over 100%
- Late deliveries reduced from 40% to 10%

**Tech Stack:** Python, OR-Tools, Kepler, Streamlit

---

## In-house Routing Engine

Built routing engine to replace third-party service, offering greater flexibility and incorporating 50+ real-life constraints.

**The Problem:**
Multi-Pickup Multi-Delivery Time Window Constraint Vehicle Routing Problem (VRP)

**Development Journey:**
- Started as self-initiated PoC using Google Scripts
- Run by control tower initially
- Success led to full engineering collaboration
- Built comprehensive logistics services suite

**Multi-Objective Optimization:**
- Minimize total distance
- Balance load across vehicles
- Ensure on-time deliveries
- Respect constraints: vehicle capacity, driver shifts, time windows, pickup/delivery sequencing

**Impact:**
- Vehicle utilization increased by 50%
- Costs reduced by 30%

**Tech Stack:** OR-Tools, Python, Google Maps API, Google App Scripts, Kepler

---

## Fleet Planner Model

Optimized vehicle combinations from third-party transport partners.

**Key Considerations:**
- Different truck types
- Payment methods: monthly subscriptions vs. ad-hoc on-demand
- First-mile, mid-mile, and last-mile deliveries

**Approach:**
- ARIMA for time series forecasting of customer demand
- Constraint programming for optimal fleet determination
- Uber-like system for auto drivers in last-mile

**Business Questions Answered:**
- How many trucks to contract monthly?
- What mix of vehicle types is optimal?
- When to use ad-hoc vehicles vs. committed fleet?

**Tech Stack:** ARIMA, Constraint Programming (OR-Tools)

---

## Other Work

### Time Series Forecasting for Produce
Conducted forecasting for major fruits and vegetables using ARIMA models to predict supply and demand patterns.

### Logistics Services Suite Enhancement
- Integrated third-party APIs for India toll fees and location services
- Calculated variable costs and enabled tracking
- Defined KPIs for routing and fleet planning services
- Enabled control tower edits for on-ground operations

### Fraud Detection
Discovered ongoing fraud by truck drivers:
- Matched truck GPS tracking data with NHAI toll data
- Identified drivers submitting fake toll amounts
- Caught drivers taking alternative, cheaper routes

### Reverse Logistics
Designed reverse logistics models including crate collection from customers.

**Tech Stack:** ARIMA, Third-party APIs, Data Analysis
