# Phase 1: Ideation Phase

## 1. Project Title
**Electric Vehicle Market Performance & Insights**

## 2. Problem Statement
The global electric vehicle (EV) automotive market is undergoing rapid growth, yet automotive manufacturers, operational planners, and market analysts struggle with data silos. Critical market telemetry—such as driving range efficiency, battery chemistries (LFP, NMC, NCA), pricing tiers, and regional customer feedback—is fragmented across legacy storage systems. Without a centralized business intelligence platform, stakeholders cannot evaluate multi-dimensional performance metrics, forecast demand trends, or identify optimization pathways for future electric mobility rollouts.

## 3. Empathy Map Canvas
### Target User: Corporate EV Strategy Director & BI Manager
- **Says:** 
  - "We need a centralized platform to visualize global EV sales volume alongside technical battery benchmarks."
  - "Extracting insights from multi-gigabyte flat files takes days instead of seconds."
- **Thinks:** 
  - "Which battery chemistry offers the best trade-off between driving range and cycle life for consumer models?"
  - "Are our competitors pricing lower-tier models more aggressively in emerging geographic clusters?"
- **Does:** 
  - Cross-examines monthly sales reports against regional dealership inventory.
  - Reviews battery chemistry safety and lifespan indices for upcoming vehicle launches.
- **Feels:** 
  - Overwhelmed by fragmented datasets and disconnected spreadsheets.
  - Pressured to make rapid, multi-million-dollar R&D capital investments backed by concrete data.

## 4. Brainstorming & Idea Prioritization
### Brainstormed Ideas:
1. Aggregate multi-source EV records into a structured relational data model.
2. Formulate optimized SQL aggregation queries for manufacturer volume and battery type breakdown.
3. Design an executive 7-to-9 visual interactive Tableau dashboard with dynamic slicers.
4. Integrate Tableau Public visualizations within a lightweight Flask web interface for zero-friction browser presentation.

### Idea Prioritization Matrix:
| Group No. | Final Idea | Feasibility | Importance | Priority | Selected |
| :--- | :--- | :--- | :--- | :--- | :--- |
| G-01 | Relational SQL ingestion & data cleaning pipeline | High | High | High | Yes |
| G-02 | Executive interactive Tableau dashboard & story points | High | High | High | Yes |
| G-03 | Flask web application wrapper for dashboard presentation | High | Medium | Medium | Yes |
