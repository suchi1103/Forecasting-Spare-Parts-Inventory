# Forecasting-Spare-parts-inventory
 AI-powered Spare Parts Inventory Forecasting system using MySQL &amp; Python to predict vehicle service demand and achieve Just-In-Time (JIT) management.


# 🚗 Vehicle Service Center: Spare Parts Inventory Forecasting System

An end-to-end data science and machine learning pipeline designed to optimize spare parts inventory management in automotive service centers. By extracting and analyzing **28,484 historical service transaction records** from a central **MySQL database**, this system predicts future component demand. 

The ultimate objective of this system is to transition service operations toward a **Just-In-Time (JIT)** inventory framework—ensuring critical replacement parts are exactly where they need to be, right when a customer pulls into the service bay, while minimizing warehouse storage costs.

---

## 🎯 Project Objectives

*   **Database Ingestion:** Securely extract operational service center data directly from a relational MySQL database.
*   **Data Sanitation:** Perform rigorous preprocessing and cleaning to resolve data inconsistencies and handle missing values across transaction blocks.
*   **Exploratory Data Analysis (EDA):** Conduct deep analytical visualizations to identify hidden seasonal patterns and usage trends in spare parts consumption.
*   **Machine Learning Modeling:** Develop predictive machine learning models to map parts demand against mileage and vehicle behavior.
*   **Time-Series Forecasting:** Implement statistical time-series forecasting techniques to analyze and project future long-term demand trends.
*   **JIT Implementation:** Support service centers in achieving Just-In-Time (JIT) standards to reduce inventory holding and storage costs while ensuring parts availability.

---

## 📊 Dataset & Feature Description

The system processes a dataset containing **28,484 operational records** consisting of 7 core engineering attributes:

| # | Feature Name | Data Type | Structural Description |
|---|---|---|---|
| **1** | `invoice_date` | Object (Date/Time) | The date when the service invoice was generated after maintenance completion. Tracks when parts were officially billed. |
| **2** | `job_card_date` | Object (Date/Time) | The date when the service request or job card was created. Indicates when the servicing process began. |
| **3** | `business_partner_name` | Object (Categorical) | The name of the customer or organization that owns the vehicle being serviced. |
| **4** | `vehicle_no` | Object (Identifier) | Unique vehicle registration number used as a core key for tracking lifetime maintenance history. |
| **5** | `vehicle_model` | Object (Categorical) | The specific model of the vehicle. Dictates the specialized spare parts and maintenance procedures required. |
| **6** | `current_km_reading` | Integer (Numerical) | Odometer reading of the vehicle at the time of servicing. Crucial for correlation against component wear thresholds. |
| **7** | `invoice_line_text` | Object (Text/Cat) | Detailed description of the specific spare parts or service items consumed during the vehicle servicing. |

---

## 🧠 Importance of Inventory Forecasting

Maintaining an un-optimized warehouse layout causes severe operational bottlenecks. Implementing predictive data analytics yields major supply chain advantages:
*   📉 **Cost Containment:** Dramatically reduces inventory holding, depreciation, and warehouse storage costs.
*   🚫 **Shortage Prevention:** Eliminates service bay bottlenecks and part stockouts.
*   ⚡ **Operational Productivity:** Boosts technician efficiency by ensuring components are available on demand.
*   🤝 **Customer Satisfaction:** Enhances customer retention rates by mitigating vehicle repair and turnaround delays.

---

.  **Extraction:** Designing optimized SQL queries to fetch clean relational records across service tables.
2.  **Feature Engineering:** Converting object datetime strings into computational index intervals and restructuring text descriptions into uniform part categories.
3.  **Visual Analytics:** Mapping consumption frequency histograms, tracking mileage-to-wear ratios, and running structural seasonality checks.
4.  **Predictive Pipelines:** Training regression frameworks and time-series forecasting models to compute demand limits.
5.  **Statistical Diagnostics:** Assessing model reliability through error metrics (MAE, RMSE) to guarantee safe deployment profiles inside active service centers.


## 🔭 Scope of Work

