# Phase 2: Requirement Analysis

## 1. Customer Journey Map
| Phase of Journey | Stage 1: Data Discovery & Ingestion | Stage 2: Exploration & BI Modeling | Stage 3: Strategic Executive Decisions |
| :--- | :--- | :--- | :--- |
| **Actions** | Ingest 200,000 raw EV records into structured tables; clean null and duplicate entries. | Build calculated metrics and interactive charts covering volume, battery life, and ratings. | Filter by country and manufacturer to determine R&D budget allocation and pricing strategy. |
| **Touchpoints** | Snowflake / SQL Database, CSV Datasets, CLI. | Tableau Desktop, Calculated Fields, Visual Worksheets. | Interactive Flask Web Interface, Executive PDF Reports. |
| **User Thoughts** | "Ensure data types, primary keys, and ranges are strictly normalized." | "Which visualizations convey regional market share and battery lifecycle most clearly?" | "We now have actionable intelligence to launch competitive hatchback models." |
| **User Feelings** | Analytical and cautious about data purity. | Engaged, discovering key manufacturer trends. | Confident, empowered with data-backed market clarity. |
| **Process Ownership** | Data Engineer / Analytics Engineer | BI Analyst / Data Visualization Specialist | EV Strategy Director / Chief Technology Officer |
| **Opportunities** | Automate ETL pipelines to handle periodic telemetry imports seamlessly. | Create drill-down filters by vehicle category and battery chemistry. | Export live presentation cards directly into executive strategy reviews. |

## 2. Solution Requirements
### Functional Requirements (FR)
- **FR-1 (Data Access & Integration):** Load and parse over 200,000 vehicle records across 39 feature attributes.
- **FR-2 (Data Processing & Hygiene):** Handle null values, eliminate duplicate vehicle IDs, and standardize categorical strings.
- **FR-3 (Business Analytics & Calculations):** Generate aggregation measures for total sales volume, average customer satisfaction scores, and battery cycle life.
- **FR-4 (Visual Dashboards):** Provide a responsive, multi-chart Tableau layout with synchronized filtering across manufacturer, year, and vehicle type.

### Non-Functional Requirements (NFR)
- **NFR-1 (Usability):** Zero-friction UI allowing non-technical leaders to filter and drill down into segments in under 3 clicks.
- **NFR-2 (Security):** Read-only data consumption protecting source records from unauthorized table alteration.
- **NFR-3 (Reliability):** 100% calculation consistency between underlying SQL queries and Tableau extract measures.
- **NFR-4 (Performance):** Dashboard interaction and visual filter responsiveness under 500 milliseconds.
- **NFR-5 (Scalability):** Schema capability to absorb additional vehicle models and regional datasets without redesign.

## 3. Technology Stack & Justification
| S.No | Component | Technology Selected | Justification / Purpose |
| :--- | :--- | :--- | :--- |
| 1 | Query / Manipulation Language | SQL / Python | High performance for data transformation, aggregation, and filtering across large tabular datasets. |
| 2 | Data Warehouse / Storage | Snowflake / Relational SQL | Enterprise-grade cloud storage offering schema scalability, indexing, and high query concurrency. |
| 3 | Business Intelligence Platform | Tableau Desktop / Public | Industry benchmark for building rich, interactive multi-variable visualizations and storytelling. |
| 4 | Web Framework | Python Flask | Lightweight micro-framework enabling rapid deployment and web embedding of BI dashboards. |
| 5 | Version Control | Git / GitHub | Secure version tracking, documentation hosting, and open-source project collaboration. |
