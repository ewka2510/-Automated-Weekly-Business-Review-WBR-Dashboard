# Automated Weekly Business Review (WBR) Dashboard

## 📌 Project Overview
This project delivers an automated Business Intelligence workflow that transforms raw, unformatted operational logs into a polished, data-driven **Weekly Business Review (WBR)** dashboard. 

Built using Microsoft's Modern BI stack (**Excel, Power Query, and Power BI**), this solution processes data from two distinct operational platforms (Ticketing and Telephony). It eliminates manual reporting errors, standardizes key performance indicators (KPIs), and provides team stakeholders with dynamic, scannable insights every Monday morning.

---

## ⚡ Key Features & Technical Highlights

* **Multi-Source Data Ingestion:** Seamlessly connects to and extracts raw data exported from two separate operational systems (Support Ticket logs and Call Center telephony logs).
* **Automated ETL Pipeline (Power Query):** 
  * Built a repeatable data transformation pipeline to clean, denormalize, and merge disparate datasets.
  * Automated data type casting, error handling, and conditional column creation.
  * Structured time-series data to aggregate individual logs into standardized daily and weekly operational views.
* **Smart Data Visualization & Conditional Formatting:**
  * **Dynamic Visual Anchors:** Implemented automated conditional formatting based on strict business logic.
  * **Color-Coded Target Tracking:** Instantly flags underperforming metrics in soft red/orange and visually rewards successful targets in green, allowing stakeholders to identify operational bottlenecks within seconds.
  * **Dual-Track Reporting:** Features side-by-side performance tracking for **Case Management** and **Telephony Performance** with integrated trend charts to spot weekly volume peaks.

---

## 🛠️ Tech Stack & Skills Demonstrated

* **Data Extraction & Transformation:** Power Query (M formula language concepts for data shaping and merging).
* **Data Modeling & Analytics:** Microsoft Excel / Power BI (KPI definition, automated calculations, and architecture design).
* **Business Intelligence (BI) Layout:** Dashboard UX/UI design, conditional formatting, and interactive data storytelling.

---

## 📊 Data Architecture & Metrics Tracked

The automated pipeline processes raw files into two main strategic areas:

### 1. Case Management Track
Tracks the lifecycle of customer support tickets against dynamic time-to-resolve (TTR) targets:
* **Volume Analysis:** Monitoring Inbound vs. Outbound distribution.
* **Quality Control:** Tracking the `Case Reopened Rate` (Target: <6%).
* **SLA Compliance:** Dual-layer monitoring for `Simple Cases` (6h TTR, Target: 90%) and `Complex Cases` (12h TTR, Target: 85%).

### 2. Telephony Performance Track
Monitors live queue efficiency and communication responsiveness:
* **Speed of Answer:** `SLA 20 sec` tracking to ensure rapid customer connection (Target: 90%).
* **Queue Leakage:** Monitoring `Missed Calls >20s` and `Abandoned Calls` to maintain a strict threshold of <3%.
