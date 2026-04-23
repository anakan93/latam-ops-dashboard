# 📊 LATAM Operations Dashboard — Power BI

A 4-page Power BI operational intelligence dashboard built to monitor data reporting compliance, account volumes, analyst performance, and sociodemographic data coverage across 10 Latin American countries.

> **Context:** Inspired by real operational dashboards built during my role as Senior Data Analyst at TransUnion LLC (2022–2024), where I was responsible for LATAM region reporting visibility and decision-making tools.

![PowerBI](https://img.shields.io/badge/Power%20BI-Desktop-F2C811?style=flat-square&logo=powerbi)
![DAX](https://img.shields.io/badge/DAX-Measures-blue?style=flat-square)
![Data](https://img.shields.io/badge/Data-Simulated%20LATAM-green?style=flat-square)

---

## Dashboard Pages

### Page 1 — Operations Overview
Answers: *Which countries are on time? Which are late? What's the overall compliance trend?*
- Compliance rate KPI card
- Country status table with conditional formatting (green/red)
- Monthly compliance trend line chart
- On Time vs Late donut chart
- Slicer by month

### Page 2 — Account Volume
Answers: *How many accounts does each country have? How is volume growing over time?*
- Total/Active/New/Closed account KPI cards
- Accounts by country horizontal bar chart
- Account volume trend area chart (Jan–Jun 2024)
- Active vs Inactive stacked bar by country

### Page 3 — Analyst Performance
Answers: *Which analysts are meeting their deadlines? Who has the most late submissions?*
- Analyst summary table with conditional formatting
- On-time rate by analyst column chart (with 90% target line)
- Late submissions over time per analyst line chart
- Workload distribution donut chart

### Page 4 — Sociodemographic Coverage
Answers: *How complete is our sociodemographic data per country? Are we meeting the 85% coverage target?*
- Avg coverage %, data quality score, countries above target KPI cards
- Coverage by country bar chart (with 85% target line)
- Field-level breakdown (age, gender, income, employment, education) by country
- Coverage vs data quality scatter plot (bubble size = account volume)
- Coverage trend over time by country

---

## Dataset

The dataset (`latam_operations_data.csv`) contains **60 rows** representing monthly operational snapshots for **10 countries** across **6 months** (Jan–Jun 2024).

**Countries covered:** Mexico, Brazil, Colombia, Argentina, Chile, Peru, Ecuador, Costa Rica, Guatemala, Dominican Republic

**Fields include:**
- Reporting compliance (submission dates, days late, status)
- Account volumes (total, active, new, closed)
- 7 sociodemographic coverage fields per country (age, gender, income, employment, education, marital status, address, phone)
- Overall coverage % and data quality score

> ⚠️ **Note:** All data in this repository is simulated for portfolio purposes. No real TransUnion data is used.

---

## DAX Measures Used

| Measure | Purpose |
|---|---|
| `Compliance Rate %` | % of reports submitted on time |
| `Avg Days Late` | Average days past deadline (late submissions only) |
| `Total Accounts` | Sum of all credit bureau accounts |
| `Account Growth %` | Net growth rate (new - closed / total) |
| `Avg Socio Coverage %` | Average sociodemographic data completeness |
| `Countries Above 85% Coverage` | Count of countries meeting coverage target |
| `Analyst On Time Rate %` | Per-analyst compliance rate |

Full DAX code available in `POWERBI_BUILD_GUIDE.md`.

---

## How to Open

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Download `LATAM_Operations_Dashboard.pbix`
3. Open in Power BI Desktop
4. All data is embedded — no external connections needed

If you want to rebuild from scratch, follow the step-by-step guide in `POWERBI_BUILD_GUIDE.md`.

---

## Screenshots

> Add screenshots to the `/screenshots` folder after building in Power BI Desktop.

| Page | Preview |
|---|---|
| Operations Overview | `screenshots/page1-overview.png` |
| Account Volume | `screenshots/page2-accounts.png` |
| Analyst Performance | `screenshots/page3-analysts.png` |
| Sociodemographic Coverage | `screenshots/page4-sociodemographic.png` |

---

## Skills Demonstrated

- Power BI report design (4-page navigation, consistent theme)
- DAX measure writing (CALCULATE, FILTER, DIVIDE, SUMMARIZE)
- Conditional formatting for operational status indicators
- KPI card design and business metric visualization
- Scatter plot with multi-dimension encoding (x, y, size, color)
- Real-world business context: credit bureau operations, LATAM region

---

## Author

**Andres Vargas**  
Master of Information Technology — ICMS, Sydney (2026)  
Former Senior Data Analyst — TransUnion LLC (2022–2024)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://linkedin.com/in/andres-vargas)
[![GitHub](https://img.shields.io/badge/GitHub-Profile-black?style=flat-square&logo=github)](https://github.com/anakan93)
