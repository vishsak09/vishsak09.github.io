---
layout: default
title: Shadowfax
period: 2021-2022
---

# Shadowfax (2021-2022)

## Hyperlocal Allocation System Refactoring

Led the refactoring of the hyperlocal allocation system, specifically enhancing the serviceability and routing engine components. This involved utilizing Python, Google OR-Tools, and Golang to improve the efficiency and performance of the allocation process.

The refactoring focused on making the system more modular, scalable, and maintainable while improving the core algorithms that determine which delivery partners are assigned to which orders based on location, capacity, and real-time availability.

**Tech Stack:** Python, Google OR-Tools, Golang

## Wavenet-based Time Series Prediction Model

Designed, developed, and successfully deployed a Wavenet-based time series prediction model into production for predicting service requests volume per client. This model significantly improved peak accuracy from 70% to 90%, leveraging Python, TensorFlow, scikit-learn, and statsmodels for enhanced forecasting capabilities.

The Wavenet architecture was chosen for its ability to capture complex temporal patterns and dependencies in the data. Unlike traditional time series methods, Wavenet's deep learning approach could learn from historical patterns at multiple time scales, making it particularly effective for capturing both daily patterns and longer-term trends.

Accurate forecasting of service requests was critical for capacity planning, allowing Shadowfax to ensure sufficient delivery partners were available during peak periods while avoiding over-allocation during slower times. The 20-percentage-point improvement in peak accuracy translated directly to better resource utilization and service quality.

**Tech Stack:** Python, TensorFlow, scikit-learn, statsmodels

## Data Science Platform Development

Worked closely with the engineering team to build a robust Data Science platform designed for the real-time training and serving of Deep Learning (DL) models. The platform's tech stack included Python, PySpark for data processing, Redis for caching, and AWS S3 buckets for storage.

The platform enabled data scientists to develop, train, and deploy models without deep engineering expertise, while ensuring models could be served at scale with low latency. This infrastructure was critical for deploying the Wavenet forecasting model and other ML systems in production.

**Tech Stack:** Python, PySpark, Redis, AWS (S3 buckets)

## Ad-hoc Tasks for Allocation Metric Improvement

Provided support to leadership on various ad-hoc tasks focused on improving key allocation metrics, contributing to strategic decision-making and operational enhancements. This included analyzing allocation patterns, identifying bottlenecks, and proposing algorithmic improvements to increase the percentage of orders successfully allocated to delivery partners.
