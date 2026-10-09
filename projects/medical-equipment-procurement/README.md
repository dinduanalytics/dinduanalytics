# Medical Equipment Procurement Analysis

> A business-focused analysis of medical equipment procurement across hospitals, examining spending, equipment condition, maintenance, installation costs, supplier geography, and delivery performance.

**Author:** Nwaba Chimdindu  
**Tools:** Microsoft Excel · Power Query · PivotTables · Dashboarding  
**Project type:** Procurement analytics / operational cost analysis

---

## Project Overview

Hospitals depend on reliable medical equipment, timely supplier deliveries, and effective cost management. This project explores a procurement dataset containing equipment, hospital, supplier, cost, delivery, warranty, and condition information.

The objective is to turn the dataset into a useful view of procurement spending and operational performance, helping stakeholders investigate where costs are concentrated and where supplier or equipment follow-up may be needed.

## Business Questions

The analysis is structured around these seven questions from the project brief:

1. **Which hospitals spend the most on equipment procurement?**
2. **How is equipment condition distributed across departments?** Which areas may need upgrades?
3. **How do maintenance costs vary by equipment type?** Which equipment types are most and least costly to maintain?
4. **What is the average delivery time for equipment from different suppliers?**
5. **Which states have the highest installation costs for medical equipment?**
6. **What proportion of equipment suppliers comes from each country?**
7. **How does equipment condition vary with installation costs?**

Together, these questions address procurement efficiency, cost management, supplier performance, and equipment lifecycle management.

## Dataset

The supplied workbook contains **260 records** and 19 fields in the Procurement Data worksheet.

| Field group | Examples |
|---|---|
| Hospital and location | Hospital, State, Location, Department |
| Equipment | Equipment, Quantity, Equipment Condition, Warranty Period (Months) |
| Procurement and lifecycle costs | Unit Price, Maintenance Cost (USD/year), Installation Cost (USD) |
| Supplier information | Supplier, Supplier Country, Supplier Contact, Supplier Phone, Supplier Email |
| Delivery timeline | Date Ordered, Date Delivered |

### Data handling note

The source workbook contains supplier contact names, phone numbers, and email addresses. Before publishing the raw workbook publicly, these fields should be removed or anonymised. This project page documents the analysis without exposing those contact details.

## Analytical Approach

1. **Understand the data** — review the fields and map them to the business questions.
2. **Prepare the data** — check data types, missing values, text consistency, and date fields.
3. **Create analytical measures** — define procurement spend, installation costs, maintenance costs, and delivery days consistently.
4. **Summarise and compare** — group results by hospital, department, equipment, supplier, state, and supplier country.
5. **Visualise performance** — use KPI cards and comparative charts to make cost and operational patterns easier to interpret.
6. **Translate results into action** — connect findings to practical procurement, supplier-management, and equipment-planning questions.

## Metric Definitions

To keep the analysis reproducible, document the exact formulas used in the workbook:

- **Procurement spend:** quantity multiplied by unit price, unless the dashboard explicitly defines procurement cost differently.
- **Delivery time (days):** date delivered minus date ordered.
- **Maintenance cost:** annual maintenance cost as provided in the dataset.
- **Installation cost:** installation cost as provided in the dataset.
- **Supplier distribution:** supplier records grouped by supplier country; state whether the visual counts records, suppliers, or equipment units.

The metric definitions should match the formulas and aggregation choices used in the final dashboard.

## Dashboard

The dashboard for this project is part of the visual portfolio. It focuses on procurement costs, high-spending hospitals, equipment types, supplier performance, installation costs, and operational recommendations.

> **Dashboard preview:** add the exported dashboard image to this repository as images/medical-procurement-dashboard.png, then embed it here.

<!-- Replace this note with:
![Medical Equipment Procurement Dashboard](images/medical-procurement-dashboard.png)
-->

## Findings and Recommendations

The final published version should include findings directly verified against the workbook/dashboard, followed by recommendations tied to those findings. Avoid treating a chart pattern as a causal explanation without further evidence.

Useful decision areas to evaluate include:

- Reviewing hospitals or states with the highest cost totals.
- Investigating departments with a higher share of equipment in poor condition.
- Comparing maintenance costs by equipment type before planning lifecycle budgets.
- Reviewing supplier delivery performance using consistently calculated delivery days.
- Evaluating supplier-country concentration as a sourcing-risk question.
- Comparing installation costs across equipment condition groups while accounting for equipment type and price.

*These are investigation and decision areas, not claims that the dataset has already established a particular cause.*

## Project Files

| File | Purpose |
|---|---|
| README.md | Project overview, questions, method, and documentation |
| Data Description.pdf | Original data description and business questions |
| Procurement Dataset.xlsx | Source workbook — sanitise supplier contact details before public release |
| Dashboard image | Visual result — add an exported image to images/ |
| Walkthrough video | Optional demonstration — add a public link or a compressed file if appropriate |

## Limitations

- The dataset describes recorded procurement and equipment attributes; it does not by itself establish why a hospital incurred a cost or why equipment is in a particular condition.
- Delivery comparisons should account for missing or invalid dates and should use a consistent definition of delivery time.
- Cost comparisons may be affected by differences in equipment type, quantity, unit price, and installation requirements.
- Supplier-country distribution depends on whether the analysis counts records, unique suppliers, or units purchased; the chosen definition should be stated.

---

## Summary

This project demonstrates a practical analytics workflow: translating procurement questions into measurable metrics, organising operational data, comparing costs and delivery performance, and presenting the results in a dashboard designed to support decisions.
