# Phase 5: Project Development Phase

## 1. Data Cleaning & Preparation
- **Null Value Treatment:** Verified that primary keys (`vehicle_id`) contain zero nulls. Missing numeric values in optional features were handled via mean imputation.
- **Deduplication:** Applied primary key indexing and unique constraints on `vehicle_id` to eliminate redundant records.
- **Categorical Standardization:** Cleaned vehicle category strings, battery chemistries (`LFP`, `NMC`, `NCA`), and country names for uniform aggregation.

## 2. Visualizations Implemented in Tableau
1. **EV Market Performance at a Glance (KPI Metric Cards):**
   - Total Manufacturers: 200
   - Total EV Models: 17,980
   - Total Annual Sales: $1,550.7M Units
   - Average Customer Satisfaction: 4.0 / 5.0
   - Average Driving Range: 324.54 KM
   - Average Battery Capacity: 78.2 kWh
2. **EV Category Performance & Distribution:** Vertical bar chart categorizing market distribution across Hatchbacks, SUVs, and Scooters.
3. **Market Share by Manufacturer:** Horizontal bar chart highlighting volume leadership among global automotive brands.
4. **Customer Rating Records by EV Category:** Treemap/Heatmap detailing customer satisfaction across market segments.
5. **Annual EV Sales Trend by Model Year:** Multi-year dual-axis line chart illustrating rapid post-2020 adoption acceleration.
6. **Battery Technology Market Share:** Donut chart evaluating volume split between LFP, NMC, and NCA chemistries.
7. **Electric Vehicle Distribution by Manufacturing Country:** Filled choropleth map highlighting production density across China, North America, and Europe.

## 3. Data Story: Global EV Manufacturing Footprint
- **Scene 1 (Global Capacity Overview):** Details global geographic concentration and regional assembly volume.
- **Scene 2 (Manufacturing Density Hubs):** Highlights key supplier hubs and localized battery cell production facilities.
- **Scene 3 (Supply Chain Resilience):** Assesses how geographic concentration affects geopolitical supply chain risks.
