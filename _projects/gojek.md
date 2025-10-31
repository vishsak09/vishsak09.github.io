---
layout: default
title: Gojek
period: 2022-Present
---

# Gojek (2022-Present)

## GOTO Logistics

### Routing Engine Leadership & Multi-Objective Strategy

Led the routing engine team, introducing a multi-objective routing strategy that successfully replaced a third-party routing service (Locus), demonstrating superior efficiency in benchmarks. The multi-objective approach allowed us to optimize for multiple goals simultaneously: minimizing total distance, balancing load across drivers, ensuring on-time deliveries, and reducing operational costs.

Collaborated with the engineering team to reduce the latencies of internal services by over 90% through the implementation of Redis-based caching and parallel calls for map services. This optimization was critical for making the routing engine practical in production, where route calculations need to happen in real-time as new orders arrive.

The routing engine utilized Python and Google OR-Tools to solve complex vehicle routing problems at scale, with scikit-learn used for ML-based feature engineering and prediction components that enhanced the optimization.

**Tech Stack:** Python, Google OR-Tools, scikit-learn, Redis

### Simulation Engine Development

Developed a versatile simulation engine that empowered decision scientists to conduct various use-case-based simulations. This tool was instrumental for the business team in determining efficient configurations for the routing engine across different service types and service areas.

The simulation engine allowed teams to answer questions like: What happens to delivery times if we add more vehicles? How does changing the time window constraints affect utilization? What's the optimal way to configure routing for a new service area? By running simulations before deploying changes, we could make data-driven decisions and avoid costly mistakes.

### Warehouse Algorithms

Focused on automating various warehouse operations by developing advanced algorithms. This included a picking algorithm utilizing Constraint Programming and Reinforcement Learning, and an optimal packing algorithm employing Constraint Programming and Transformers.

The picking algorithm optimized the sequence in which warehouse workers collect items from shelves, minimizing walking distance while respecting constraints around item locations, order priorities, and worker capacity.

The packing algorithm served two purposes: helping the business team decide what box sizes to stock, and helping warehouse operations determine the optimal packaging sequence and box selection for each order. The Transformer-based approach could learn from historical packing data to make intelligent predictions about which items would fit best together.

Additionally, worked with the warehouse team on initial analyses for human capacity planning algorithms to optimize staffing levels based on predicted order volumes.

**Tech Stack:** Constraint Programming, Reinforcement Learning, Transformers

## Gojek Marketplace

### Improving BCR with Simulation Engine

Achieved a ~10% improvement in Booking Conversion Rate (BCR) by leveraging the simulation engine to identify and implement optimal configurations at a granular, zone-level within the city.

Different zones have different supply-demand dynamics, traffic patterns, and customer behaviors. By optimizing configurations zone-by-zone rather than using city-wide settings, we could significantly improve the match rate between riders and drivers, leading to more successful bookings.

### Allocation Engine Development

Developed a sophisticated Batch Allocation Model based on the Min-Cost Max-Flow problem, capable of handling over 5 million orders daily. This replaced an earlier greedy algorithm that operated on a FIFO (First-In-First-Out) mechanism, leading to increased allocation efficiency.

The Min-Cost Max-Flow formulation allowed us to find globally optimal allocations across batches of orders and drivers, rather than making myopic decisions order-by-order. This approach considers future demand and supply when making allocation decisions, leading to better overall system performance.

Additionally, created ensemble models to generate customized scores for order-driver pairs, representing the probability of conversion. These ML models considered features like historical acceptance rates, distance, driver preferences, and real-time context to predict which driver-order pairings were most likely to succeed.

The tech stack included XGBoost for the ML models, Python for model training and orchestration, Golang for the production allocation service, and Google OR-Tools for solving the optimization problem.

**Tech Stack:** XGBoost, Python, Golang, Google OR-Tools

## Migration from Google Cloud to Multi-Cloud Environment

Successfully led the migration of one of Gojek's largest data pipelines and models from Google Cloud to a multi-cloud environment (Alibaba and Tencent). This project involved migrating over 200 BigQuery queries to MaxCompute (including SQL conversion), 50+ real-time data streams from Kafka, and 30+ model training and deployment tasks, encompassing more than 20TB of data, all without any downtime.

The migration was particularly complex because it involved moving to a two-cloud system: real-time data from Tencent, historical data from Alibaba Cloud. This required careful coordination and validation to ensure data consistency across clouds.

Collaborated closely with data engineering to validate and debug data retrieval techniques in the new system, writing over 100 scripts for data validation, load testing, and migration. These scripts ensured that every query, stream, and model produced identical results in the new environment before cutover.

The zero-downtime requirement meant we had to build parallel systems, validate thoroughly, and execute a carefully orchestrated cutover. This project demonstrated the importance of comprehensive testing, incremental migration, and having robust rollback plans.

**Tech Stack:** BigQuery, Kafka, MaxCompute, Python, Alibaba Cloud, Tencent Cloud

## Order-Level Incentive to Driver

Working on a new project to implement customized and personalized incentives for drivers upon completing orders. This initiative aims to enhance trust and Booking Conversion Rate (BCR) for loyal customers in timely order fulfillment, and to provide greater benefits for loyal drivers on the platform.

The challenge is to determine the optimal incentive amount for each order-driver pair, balancing multiple objectives: maximizing conversion rates, rewarding loyalty, controlling costs, and maintaining fairness. The models involved include Constraint Optimization for the allocation and incentive optimization problem, XGBoost for predicting driver behavior and conversion probability, and Reinforcement Learning for learning optimal incentive policies over time.

**Tech Stack:** Constraint Optimization, XGBoost, Reinforcement Learning
