# Phase 4: Project Planning Phase

## 1. Product Backlog & Sprint Schedule
| Sprint | Functional Requirement (Epic) | User Story Number | User Story / Task Description | Story Points | Priority | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Sprint-1** | Data Pipeline Setup | USN-01 | Ingest raw `ev_market_train` dataset into relational database tables. | 5 | High | Completed |
| **Sprint-1** | Data Hygiene & Validation | USN-02 | Execute SQL scripts to remove null values and deduplicate vehicle entries. | 5 | High | Completed |
| **Sprint-2** | Analytics Engine | USN-03 | Write SQL queries for aggregate volume, average driving range, and battery type share. | 8 | High | Completed |
| **Sprint-2** | Visual Design | USN-04 | Build worksheets for 7 primary visuals (KPI cards, bar charts, line trends, maps). | 8 | High | Completed |
| **Sprint-3** | Executive Dashboard | USN-05 | Combine visual worksheets into a unified Tableau dashboard with dynamic slicers. | 5 | High | Completed |
| **Sprint-3** | Data Storytelling | USN-06 | Construct Tableau Story "Global EV Manufacturing Footprint" analyzing supply chains. | 5 | Medium | Completed |
| **Sprint-4** | Web Application Integration | USN-07 | Create Flask backend (`app.py`) and frontend template (`index.html`) to embed visuals. | 6 | Medium | Completed |
| **Sprint-4** | Final Testing & Audit | USN-08 | Validate filter responsiveness, write project documentation, and publish demo. | 8 | High | Completed |

## 2. Velocity & Burndown Metric
- **Total Planned Story Points:** 50
- **Sprint Duration:** 10 Days
- **Team Velocity (AV):** 
  $$\text{Average Velocity} = \frac{\text{Total Story Points Completed}}{\text{Sprint Duration}} = \frac{50}{10} = 5 \text{ points/day}$$
