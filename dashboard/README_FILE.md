## Dashboard Files

This folder contains the main Power BI dashboard implementation for the **Managed Services Performance & SLA Analytics** project, along with its static export for offline review.

### 📁 Files Included

- **Managed Services Performance and SLA Analytics.pbix**  
  The primary Power BI Desktop file containing:
  - Star schema data model (Fact & Dimensions)
  - DAX measures and KPI logic
  - All report pages and visualizations

- **Managed Services Performance and SLA Analytics.pdf**  
  A static export of the dashboard used for:
  - Quick preview without Power BI Desktop
  - Sharing with stakeholders who require read-only access

### 📊 Dashboard Coverage

The Power BI dashboard consists of four main pages:
1. **Executive Overview**  
   High-level service health check for management, including SLA compliance, incident trends, and severity distribution.
2. **Service & Operations**  
   Operational analysis focusing on SLA by service type, MTTR, and identification of process or capacity bottlenecks.
3. **Client & Region**  
   Risk analysis by client and geographic region to support proactive account management and escalation prevention.

4. **Governance & KPI Definition**  
   Data lineage, KPI definitions, calculation logic, and ownership information to ensure transparency, consistency, and audit readiness.

### 🏗️ Data Model & KPI Implementation

- Data model designed using **Star Schema**
- Central fact table: `Fact_Incident`
- Supporting dimensions: Date, Service, Client, Region, Severity
- Relationships: One-to-Many (Dimension → Fact), single direction
- KPIs implemented using **DAX measures** (not calculated columns)

### 🎯 Purpose

The dashboard is designed to:
- Monitor SLA compliance and service reliability
- Identify operational risks early
- Support executive and operational decision-making
- Provide a trusted and audit-ready analytics solution

### 📝 Notes

- The dataset used is a realistic simulation for portfolio purposes.
- The design and implementation follow enterprise Business Intelligence and data governance best practices.
