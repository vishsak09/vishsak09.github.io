---
layout: single
title: Gojek
period: 2022-Present
---

# Gojek (2022-Present)

## GOTO Logistics

### Routing Engine Leadership & Multi-Objective Strategy

Led routing engine team and replaced third-party service (Locus) with in-house solution.

**Multi-Objective Optimization:**
- Minimize total distance
- Balance load across drivers
- Ensure on-time deliveries
- Reduce operational costs

**Performance Improvements:**
- Reduced service latencies by 90%
- Implemented Redis-based caching
- Enabled parallel calls for map services
- Made real-time route calculations practical at scale

**Tech Stack:** Python, Google OR-Tools, scikit-learn, Redis

---

### Simulation Engine Development

Built simulation engine for decision scientists to run use-case-based simulations.

**Key Questions Answered:**
- What happens to delivery times if we add more vehicles?
- How does changing time window constraints affect utilization?
- What's the optimal routing configuration for new service areas?

**Value:**
- Make data-driven decisions before deploying changes
- Avoid costly mistakes
- Determine efficient configurations across service types and areas

---

### Warehouse Algorithms

Developed algorithms to automate warehouse operations.

**Picking Algorithm:**
- Optimized sequence for collecting items from shelves
- Minimized walking distance
- Respected constraints: item locations, order priorities, worker capacity
- Used: Constraint Programming + Reinforcement Learning

**Packing Algorithm:**
- Helped business team decide box sizes to stock
- Helped operations determine optimal packaging sequence
- Learned from historical packing data using Transformers
- Made intelligent predictions about item combinations

**Additional Work:**
- Human capacity planning algorithms
- Optimized staffing levels based on predicted order volumes

**Tech Stack:** Constraint Programming, Reinforcement Learning, Transformers

---

## Gojek Marketplace

### Improving BCR with Simulation Engine

Improved Booking Conversion Rate (BCR) by ~10% through zone-level optimization.

**Approach:**
- Different zones have different supply-demand dynamics, traffic patterns, customer behaviors
- Optimized configurations zone-by-zone vs. city-wide settings
- Improved match rate between riders and drivers
- Led to more successful bookings

---

### Allocation Engine Development

Built Batch Allocation Model handling 5M+ daily orders, replacing greedy FIFO algorithm.

**Min-Cost Max-Flow Approach:**
- Finds globally optimal allocations across batches
- Considers future demand and supply
- Better overall system performance vs. myopic order-by-order decisions

**ML Models:**
- Created ensemble models for order-driver pair scoring
- Predicted probability of conversion
- Features: historical acceptance rates, distance, driver preferences, real-time context
- Identified most likely successful pairings

**Tech Stack:** XGBoost, Python, Golang, Google OR-Tools

---

## Multi-Cloud Migration

Led migration from Google Cloud to Alibaba/Tencent clouds with zero downtime.

**Scale:**
- 200+ BigQuery queries migrated to MaxCompute (including SQL conversion)
- 50+ real-time Kafka data streams
- 30+ model training and deployment tasks
- 20TB+ of data

**Complexity:**
- Two-cloud system: real-time data from Tencent, historical data from Alibaba
- Required careful coordination for data consistency
- Built parallel systems and validated thoroughly

**Validation:**
- Wrote 100+ scripts for data validation, load testing, migration
- Ensured identical results before cutover
- Comprehensive testing and incremental migration
- Robust rollback plans

**Tech Stack:** BigQuery, Kafka, MaxCompute, Python, Alibaba Cloud, Tencent Cloud

---

## Order-Level Driver Incentives

Developing personalized incentive system for drivers upon order completion.

**Goals:**
- Enhance trust and BCR for loyal customers
- Provide greater benefits for loyal drivers
- Ensure timely order fulfillment

**Challenge:**
Determine optimal incentive amount for each order-driver pair while balancing:
- Maximizing conversion rates
- Rewarding loyalty
- Controlling costs
- Maintaining fairness

**Approach:**
- Constraint Optimization for allocation and incentive optimization
- XGBoost for predicting driver behavior and conversion probability
- Reinforcement Learning for learning optimal incentive policies over time

**Tech Stack:** Constraint Optimization, XGBoost, Reinforcement Learning
