---
layout: default
title: Ninjacart
period: 2019-2021
---

# Ninjacart (2019-2021)

## Logistics Control Tower KPIs & Dashboard

Analyzed end-to-end control tower operations to establish key performance indicators for daily logistics management, including truck plan creation and monitoring. Defined metrics such as Transport Performance (on-time delivery, shipment delay rate), Fleet Utilization (truck utilization), and Cost/Efficiency (cost per trolley).

Developed and implemented a Google Looker Studio dashboard, integrated with Google App Scripts, to track these KPIs effectively. The dashboard was used by leadership for key decision making across logistics operations.

**Tech Stack:** Google Looker Studio, Google App Scripts

## Supply Chain Model Change Analysis (DC to Micro-DC)

Conducted a comprehensive analysis of Ninjacart's supply chain model, transitioning from 1-2 large distribution centers (DCs) on city outskirts to a decentralized network of 15-20 smaller micro-DCs (dark stores) within cities.

My work involved determining the optimal number and location of these micro-DCs based on capacities and order volumes. This optimization, utilizing Python, OR-Tools, Kepler, and Streamlit, led to a significant increase in business operational efficiency by over 100%, reducing late deliveries from 40% to 10%.

**Tech Stack:** Python, OR-Tools, Kepler, Streamlit

## In-house Routing Engine

Created an in-house routing engine using OR-Tools and Python to overcome limitations of a third-party service, offering greater flexibility in objectives and incorporating over 50 real-life constraints. This Multi-Pickup Multi-Delivery Time Window Constraint Vehicle Routing Problem (VRP) model significantly increased vehicle utilization by over 50% and reduced costs by more than 30%.

Initially, a PoC was developed by my own initiative and run by the control tower using Google Scripts. Following its success, I collaborated with the engineering team to build a comprehensive logistics services suite, including the routing engine, fleet planner, simulation engine and relevant dashboards.

The multi-objective routing approach allowed us to balance competing objectives like minimizing distance, balancing load across vehicles, and ensuring on-time deliveries while respecting real-world constraints around vehicle capacity, driver shifts, time windows, and pickup/delivery sequencing.

**Tech Stack:** OR-Tools, Python, Google Maps API, Google App Scripts, Kepler

## Fleet Planner Model Development

Developed a sophisticated fleet planner model to optimize the combination of vehicles from various third-party transport partners, considering different truck types and payment methods (monthly subscriptions vs. ad-hoc on-demand).

This model integrated ARIMA for time series forecasting of customer demand and constraint programming to determine the optimal fleet. It was applied to both first-mile and mid-mile deliveries, with a tailored constraint programming model for last-mile deliveries to manage ad-hoc vehicles and an Uber-like system for auto drivers.

The fleet planner helped answer critical business questions: How many trucks should we contract monthly? What mix of vehicle types is optimal? When should we rely on ad-hoc vehicles vs. committed fleet? By forecasting demand patterns and optimizing fleet composition, we reduced costs while maintaining service levels.

**Tech Stack:** ARIMA, Constraint Programming using OR-Tools

## Ad-hoc Works

**Time Series Forecasting for Produce:** Conducted time series forecasting for major fruits and vegetables using ARIMA models to predict supply and demand patterns.

**Logistics Services Suite Enhancement:** Collaborated with the engineering team to enhance the logistics services suite, integrating third-party APIs for India toll fees and location services to accurately calculate variable costs and tracking. Also worked with the business team to define relevant KPIs for various services, such as routing (allowing control tower edits for on-ground operations) and fleet planning (displaying estimated cost and utilization).

**Fraud Detection:** Discovered an ongoing fraud by truck drivers by matching truck tracking (ping) data with NHAI toll data, identifying instances where drivers submitted fake toll amounts while taking alternative, less expensive routes.

**Reverse Logistics:** Worked with operations teams to design different reverse logistics models, including the collection of crates from customers.

**Tech Stack:** ARIMA, Third-party APIs, Data Analysis
