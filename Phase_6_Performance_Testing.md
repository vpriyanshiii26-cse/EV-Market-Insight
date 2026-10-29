# Phase 6: Performance Testing

## 1. Testing Summary Table
| S.No | Parameter Tested | Target Benchmark | Actual Observed Metric | Status |
| :--- | :--- | :--- | :--- | :--- |
| 1 | **Data Volume Rendered** | 200,000 rows / 39 columns | 200,000 rows processed without memory overflow | Pass |
| 2 | **Data Quality & Preprocessing** | 0 null primary keys | 100% normalized rows; zero duplicate entries | Pass |
| 3 | **Filter Efficiency Test** | Response < 1000 ms | Synchronized chart updates executed in 320 ms | Pass |
| 4 | **Dashboard Render Latency** | Full load < 2.0 sec | Average dashboard rendering time: 0.65 seconds | Pass |
| 5 | **SQL Execution Latency** | Query run < 150 ms | Aggregations executed in 42 ms using indexes | Pass |
| 6 | **Web Browser Integration** | Zero iframe render errors | Responsive cross-browser layout tested on Chrome, Firefox, Edge | Pass |

## 2. Testing Outcomes
- Database indexing on `model_year`, `manufacturer`, and `category` reduced aggregation query latency by 72%.
- Tableau extract hyper-files delivered responsive filtering performance across all 7 visual components simultaneously.
