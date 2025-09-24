# Digital Marketing Analysis & Visualization (Voila Dashboard)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/limlinaok/Digital-Marketing-Analysis-Visualization-using-Voila-/main?urlpath=voila/render/digital_marketing.ipynb)

---

### **Business Context**

Velocity Digital is a full-service digital marketing agency that specializes in managing **multi-platform advertising campaigns** across **Google Ads, Facebook, Instagram, LinkedIn, and TikTok**. Our services span the full campaign lifecycle — from **strategic planning and creative development** to **campaign execution, performance analysis, and optimization**.

Our client base is expanding rapidly, with a strong footprint in **the EU, the US, the UK, and Germany**. We serve diverse industries such as **beauty, health & wellness, IT solutions, food & beverage, and pet services**. Each client brings unique business goals, compliance requirements, and performance expectations, which underscores the need for a scalable and well-structured data environment.

As Velocity Digital scales, our growth has **outpaced our current data infrastructure**. The lack of a fully functional, centralized **data pipeline** has created several operational bottlenecks.

---

### **Data Extraction & Processing**

All insights in this dashboard are backed by a **PostgreSQL database**. The workflow is:

- 🔗 **Connect to PostgreSQL** using SQLAlchemy from Python in VS Code  
- 📑 **Write SQL queries** to extract tables such as campaign performance, client contracts, budgets, and conversions  
- 🐍 **Transform data with pandas** (grouping, joins, aggregations, percentage calculations)  
- 📈 Prepare clean DataFrames for visualization  

Example query snippet:  

```sql
SELECT COUNT(*) AS employees_count, manager
FROM employees
GROUP BY manager
ORDER BY employees_count DESC;
