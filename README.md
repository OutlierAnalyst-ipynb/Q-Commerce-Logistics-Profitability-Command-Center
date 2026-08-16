# Q-Commerce Logistics & Profitability Command Center

An end-to-end data analytics and business intelligence solution designed to simulate supply chain operations, isolate regional bottlenecks, and optimize financial margins for quick-commerce delivery fleets.

## 🛠️ Tech Stack
* **Power BI & DAX:** Advanced data modeling, What-If simulation parameters, and dynamic KPI tracking.
* **Python & Pandas:** ETL pipeline, epoch timestamp cleaning, categorical text standardization, and programmatic dataset scaling to 1M+ records.
* **SQLite & Star Schema:** Normalized relational database architecture with 1 Fact table and 6 Dimension tables optimized for high-performance querying via ODBC.

## 📊 Project Architecture & Key Features
1. **1M+ Row Data Pipeline:** Scaled baseline operational logs using Python to stress-test the VertiPaq analytics engine.
2. **Relational Star Schema:** Built an SQLite star schema (`Fact_Delivery` linked via 1-to-Many relationships to 6 explicit dimensions: Partner, Vehicle, Mode, Region, Weather, Package).
3. **What-If Simulation Engine:** Engineered DAX measures allowing operations managers to simulate fluctuating driver incentive payouts and instantly visualize their impact on profit margins.
4. **Root Cause Isolation:** Configured geospatial heatmaps and AI-driven decomposition trees to pinpoint specific operational failure points (e.g., Express deliveries failing during adverse weather).

## 🚀 Strategic Business Impact
* Identified that Express delivery modes combined with stormy weather conditions formed the primary operational failure point (~100% delay rate).
* Formulated data-driven route-throttling and partner-reallocation strategies to eliminate ~33,600 delayed orders.
* Achieved a **12% overall improvement in delivery fleet efficiency** while maintaining target profit margins.

## 📂 Project Directory Structure
```text
Q-Commerce Logistics & Profitability Command Center/
│
├── Data files/
│   ├── Delivery_Logistics.csv                     # Original 25k raw operational dataset
│   └── Updated/
│       ├── Cleaned_Delivery_Logistics_1M.csv      # Scaled 1M+ cleaned production dataset
│       └── Logistics_Command_Center.db            # SQLite Star Schema relational database
│
├── Notebooks/
│   └── ETL_StarSchema.ipynb                       # Interactive Jupyter Notebook version of the pipeline
│
├── Dashboard/
│   └── Q-Commerce_Command_Center.pbix             # Final Power BI interactive report
│
├── Dashboard_Preview.pdf                          # High-resolution PDF export for quick review
└── README.md                                      # Project documentation
