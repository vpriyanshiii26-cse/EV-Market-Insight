# Phase 3: Project Design Phase

## 1. Problem-Solution Fit Canvas
- **Customer Segment:** Global EV manufacturers, strategic investment analysts, and sustainable mobility policy makers.
- **Customer Constraints:** Disparate data schemas, high computing costs for ad-hoc analytical queries, and complex reporting tools.
- **Jobs to be Done:** Benchmark competitor range-to-price ratios, evaluate market adoption of LFP vs. NMC batteries, and forecast sales growth.
- **Triggers:** New competitor vehicle launches, government emission mandates, and fluctuating battery component costs.
- **Root Cause:** Legacy analytical workflows relied on disconnected spreadsheets that could not process high-volume vehicle telemetry efficiently.
- **Proposed Solution:** An integrated end-to-end data platform connecting sanitized database tables to high-fidelity Tableau dashboards served via a secure web portal.

## 2. Data Flow Diagram (DFD Level 0)
```text
 +---------------------+          Raw EV Telemetry Records
 |  Market Data Source | ----------------------------------------+
 +---------------------+                                         |
                                                                 v
                                                     +-----------------------+
                                                     | 1.0 Data Ingestion &  |
                                                     |     Standardization   |
                                                     +-----------------------+
                                                                 |
                                                                 v
                                                     +-----------------------+
                                                     |   D1: EV Database     |
                                                     |    (200k Records)     |
                                                     +-----------------------+
                                                                 |
                                                                 v
                                                     +-----------------------+
                                                     | 2.0 KPI Computation & |
                                                     |    SQL Aggregations   |
                                                     +-----------------------+
                                                                 |
                                                                 v
                                                     +-----------------------+
                                                     | 3.0 Tableau Analytics |
                                                     |    Dashboard & Story  |
                                                     +-----------------------+
                                                                 |
                                                                 v
 +---------------------+       Filtered Business Insights    +-----------------------+
 | Strategy Executive  | <---------------------------------- | 4.0 Flask Web Server  |
 +---------------------+                                     |     (Presentation)    |
                                                             +-----------------------+
