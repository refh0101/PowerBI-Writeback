# Power BI Write‑Back Project  
### Using Translytical Task Flows (Preview)

## 1. Introduction
This project demonstrates how to enable **write‑back functionality** in Power BI using **Translytical Task Flows** within Microsoft Fabric.  
Traditionally, Power BI is a read‑only analytics tool. With translytical task flows, end‑users can now perform direct actions on underlying data sources — such as adding, editing, or deleting records — and see those changes reflected immediately in reports.  

The project uses the **Adventure Works sample dataset** to simulate real‑world business scenarios.

---

## 2. Objectives
- Enable **write‑back capabilities** in Power BI.  
- Demonstrate how users can:
  - **Add data**: Insert new records into a database table.  
  - **Edit data**: Update existing records (e.g., status fields, annotations).  
  - **Delete data**: Remove outdated records.  
  - **Call external APIs**: Trigger workflows or update external systems.  
- Showcase integration of transactional and analytical workflows in Microsoft Fabric.

---

## 3. Tools & Platform
- **Microsoft Fabric**: Provides translytical task flow capabilities.  
- **Power BI**: Front‑end reporting and visualization tool.  
- **Adventure Works Dataset**: Sample dataset used for demonstration.  
- **External APIs (optional)**: REST endpoints for workflow integration.  

---

## 4. Translytical Task Flow Syntax Examples

### Add Data
```sql
-- Add a new customer record
INSERT INTO AdventureWorks.Customers (CustomerID, Name, Status)
VALUES (1001, 'John Doe', 'Active');
