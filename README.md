# KIIT SAP Project — Order-to-Cash (O2C) End-to-End Scenario

**Student Name:** Diya Sarkar
**Roll Number:** 23051104
**University:** KIIT University, Bhubaneswar  
**Project Topic:** Order-to-Cash (O2C) — Complete Sales Cycle (SAP SD)

---

## Project Overview

This project implements the **Order-to-Cash (O2C)** end-to-end business scenario for a fictitious Indian retail company — **Nova Mart Retail Pvt. Ltd.** — using SAP SD (Sales & Distribution) as the primary module, integrated with SAP FI (Financial Accounting) and SAP MM (Materials Management).

The O2C cycle covers the complete flow from customer inquiry to cash collection:

```
Customer Inquiry → Quotation → Sales Order (VA01)
    → Delivery (VL01N) → Goods Issue (VL02N)
        → Invoice / Billing (VF01) → Payment (F-28)
```

---

## Company: Nova Mart Retail Pvt. Ltd.

| Detail | Value |
|--------|-------|
| Industry | Multi-Category Retail |
| HQ | Mumbai, Maharashtra |
| Categories | Electronics, Clothing, Home & Living |
| Revenue (FY 2024-25) | ₹850 Crore (fictitious) |
| Stores | 18 outlets across India |
| SAP System | SAP ECC 6.0 / S/4HANA |
| Company Code | NM01 |
| Sales Organization | NMSO |

---

## Repository Contents

| File | Description |
|------|-------------|
| `Nova_Mart_Project_Report.pdf` | Full formal project report (10 sections, ~25 pages) |
| `Nova_Mart_SAP_Dataset.xlsx` | 240-row synthetic O2C sales dataset + summary analysis + 5 charts |
| `README.md` | This file |
| `KIIT_SAP_Project.zip` | Complete submission archive |

---

## Excel Workbook Structure

The Excel file (`Nova_Mart_SAP_Dataset.xlsx`) contains 4 sheets:

1. **Sales_Data** — 240 transaction rows with 22 columns (Order ID, Customer, Product, Qty, Price, Dates, Payment Status, etc.)
2. **Summary_Analysis** — Pivot-style tables: Monthly Revenue, Category Sales, Region Sales, Payment Status, Top 10 Products, Sales Rep Performance
3. **Charts** — 5 embedded charts: Monthly Revenue Bar, Category Pie, Region Bar, Payment Status Pie, Top 5 Products Bar
4. **Company_Overview** — SAP organizational structure (FI, MM, SD configuration tables)

---

## Key Findings

- **Electronics** is the dominant category (~55-60% of revenue)
- **Festive season (Oct-Nov)** drives peak monthly revenue
- **North & West regions** lead in sales volume
- **~82% payment collection rate** within agreed credit terms
- **Average O2C cycle: 35-45 days**

---

## SAP Transaction Codes Used

| T-Code | Purpose |
|--------|---------|
| VA01 | Create Sales Order |
| VL01N | Create Outbound Delivery |
| VL02N | Post Goods Issue |
| VF01 | Create Billing Document |
| F-28 | Post Incoming Payment |
| XD01 | Create Customer Master |
| MM01 | Create Material Master |
| SPRO | SAP Customizing (IMG) |
