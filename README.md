# 🍕 Pizza Delivery Operations Performance Dashboard (Power BI)

## Overview
This project presents an end-to-end analysis of pizza delivery operations using Power BI.  
The dashboard focuses on delivery performance, customer complaints, time-based demand patterns, and driver efficiency to support data-driven operational decisions.

The analysis demonstrates how structured data modeling and visualization can generate meaningful insights even from short operational time windows.

---

## Problem Statement
The business experienced:
- Inconsistent delivery times
- A noticeable volume of customer complaints
- Limited visibility into when and why complaints occur

The objective was to transform raw delivery data into clear insights that explain:
- When delays and complaints happen
- Whether complaints are linked to delivery time or other operational factors
- Which areas and drivers are most impacted

---

## Data Pipeline

### 1. Data Source
- Pizza delivery operational dataset used as part of a **Vuuma Collaboration case study**
- Time period covered: **03/10/2018 – 06/10/2018**
- Dataset includes:
  - Orders
  - Delivery timestamps
  - Preparation stages
  - Customer complaints and reasons
  - Drivers
  - Delivery areas
  - Order and delivery time attributes

> **Ethical Note:**  
> The dataset was provided for educational and analytical purposes as part of a case study.  
> While the data may be simulated or anonymized, the analytical approach, methodology, and insights demonstrated in this project reflect real-world business analytics practices and are ethically used for learning and portfolio development.

---

### 2. Data Preparation (Power Query)
- Cleaned and standardized date and time fields
- Handled missing values (e.g. complaints without stated reasons)
- Created derived columns:
  - **Time of Day categories** (Lunch, Afternoon, Evening, Late Night)
  - **Delivery Status** (On-Time vs Late)
- Converted delivery and preparation times into minutes for consistency

---

### 3. Data Modeling & Calculations (DAX)
- Created dynamic measures for:
  - Total Orders
  - Average Delivery Time
  - Total Complaints
  - On-Time Deliveries
  - Late Deliveries
- Complaint-related metrics respond dynamically to slicers and filters, enabling interactive analysis

---

### 4. Visualization (Power BI)
- Interactive operational dashboard designed for decision support
- Slicers included:
  - **Delivery Status**
  - **Pizza Size**
- All visuals update dynamically based on user selections

---

## Dashboard Preview

### Pizza Delivery Operations Overview
<img width="1182" height="673" alt="Image" src="https://github.com/user-attachments/assets/23e20673-c9ea-4218-84e1-f550578dca31" />

>  *The dashboard above shows the main operational dashboard highlighting delivery performance, complaints by time of day, and driver efficiency.*

---

## Key Metrics
- **Total Orders:** 12.77K  
- **Average Delivery Time:** 32.06 minutes  
- **Total Complaints:** 975  
- **Late Deliveries:** 7,401  
- **On-Time Deliveries:** 5,372  
- **Delivery Areas:** 6  
- **Delivery Drivers:** 7  

---

## Key Insights

### Delivery Performance
- **58% of deliveries were late**, indicating operational strain during peak periods.
- Complaints also occur during on-time deliveries, suggesting quality or expectation issues beyond delivery speed alone.

### Complaints by Time of Day
- Complaints peak during **Evening and Afternoon** periods.
- Late-night orders show fewer complaints overall, but higher sensitivity when delays occur.

### Area-Based Performance
- Certain delivery areas consistently record higher average delivery times.
- These areas may benefit from targeted staffing, routing optimization, or operational restructuring.

### Driver Performance
- Delivery performance varies significantly across drivers.
- Some drivers maintain higher on-time delivery rates under similar workloads, indicating best practices that could be replicated.

---

## Business Value
This dashboard demonstrates how data analytics can:
- Identify operational bottlenecks
- Improve customer satisfaction strategies
- Support smarter staffing and routing decisions
- Generate actionable insights even from small or simulated datasets

The project emphasizes **data interpretation, storytelling, and business decision support**, not just visualization.

---

## Tools Used
- **Power BI** – Data modeling, DAX measures, interactive dashboards  
- **Power Query** – Data cleaning and transformation  
- **Microsoft Excel** – Initial data inspection and validation  

---

## How to Explore This Project
- View the dashboard screenshots directly in this repository
- Download and open the Power BI `.pbix` file to interact with slicers and explore insights dynamically

---

## Notes
- The dataset may be simulated or anonymized as part of a case study.
- The analytical techniques and insights are applicable to real-world delivery, logistics, and operations environments.

---

## Author
Built as part of a hands-on analytics case study to strengthen practical data analysis, visualization, and business storytelling skills.
