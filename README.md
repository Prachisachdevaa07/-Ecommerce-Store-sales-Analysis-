# E-commerce Sales Data Analysis using Excel

An Excel-based analysis and interactive dashboard of 2022 online apparel sales across Indian marketplaces. The workbook takes ~31,000 raw order lines, summarises them with PivotTables, and presents the results as a one-page dashboard with charts and slicers.

---

## Highlights

| Metric | Value |
|---|---|
| Order lines analysed | 31,047 |
| Unique orders | 28,471 |
| Unique customers | 28,437 |
| Total sales | ₹21,176,377 |
| Average line value | ≈ ₹682 |
| Period covered | 4 Jan 2022 – 6 Dec 2022 |
| Delivered rate | 92.2% (28,641 lines) |

### Key findings

- **Women drive most revenue:** ₹13.56M (≈64%) vs ₹7.61M (≈36%) for men.
- **Top 5 states by sales:** Maharashtra (₹2.99M), Karnataka (₹2.65M), Uttar Pradesh (₹2.10M), Telangana (₹1.71M), Tamil Nadu (₹1.68M).
- **Channels:** Amazon leads (~35% of orders), followed by Myntra (~23%) and Flipkart (~22%). Ajio, Nalli, Meesho and Others each account for under ~6%.
- **Order status:** 28,641 delivered, 1,045 returned, 844 cancelled, 517 refunded.
- **Monthly trend:** Sales peak in March (₹1.93M, 2,819 orders) and decline steadily to ₹1.62M in December. Orders and revenue move closely together.
- **Top categories by revenue:** Set (₹10.5M), Kurta (₹4.96M), Western Dress (₹3.15M).
- **Adult women (30–49)** are the single largest age/gender segment, at about 35% of orders.

> Note: December covers only the first week of the month (data ends 6 Dec), and January starts on the 4th, so monthly comparisons at the edges are not like-for-like.

---

## Workbook structure

| Sheet | Purpose |
|---|---|
| `Ecommerce sales data analysis` | Raw data: 31,047 rows × 21 columns |
| `Sales vs Orders` | PivotTable and chart: monthly sales amount vs order count |
| `Men vs Women` | PivotTable and chart: sales split by gender |
| `Top 5 States` | PivotTable and chart: top five states by sales |
| `Order status` | PivotTable and chart: delivered / returned / cancelled / refunded |
| `Age n gender` | PivotTable and chart: share of orders by age group and gender |
| `Chanels` | PivotTable and chart: share of orders by sales channel |
| `Ecommerce sales report ` | Final dashboard combining the six charts, with slicers |

---

## Data dictionary

| Column | Description |
|---|---|
| `index` | Row number |
| `Order ID` | Order identifier (an order can span several lines) |
| `Cust ID` | Customer identifier |
| `Gender` | Men / Women |
| `Age` | Customer age (18–78) |
| `Age group` | Teenager (18–29), Adult (30–49), Senior (50–78) |
| `Date` | Order date |
| `Month` | Month abbreviation derived from `Date` |
| `Status` | Delivered, Returned, Cancelled, Refunded |
| `Channel` | Marketplace: Amazon, Myntra, Flipkart, Ajio, Nalli, Meesho, Others |
| `SKU` | Product SKU code |
| `Category` | Set, Kurta, Western Dress, Top, Saree, Ethnic Dress, Blouse, Bottom |
| `Size` | Garment size (S–XXL etc.) |
| `Qty` | Units ordered |
| `Currency` | INR for all rows |
| `Amount` | Line value in INR |
| `ship-city`, `ship-state`, `ship-postal-code`, `ship-country` | Shipping destination (all India, 50 states/regions) |
| `B2B` | TRUE for business orders (186 rows), otherwise FALSE |

---

## Method

1. **Clean the data:** standardise columns, derive `Age group` and `Month`, and check for blanks and duplicates (none found).
2. **Summarise with PivotTables:** one PivotTable per question (time, gender, geography, status, demographics, channel).
3. **Visualise:** a bar, line or pie chart on each PivotTable.
4. **Build the dashboard:** place all charts on a single report sheet and add slicers for interactive filtering.

---

## Tools

Microsoft Excel: PivotTables, PivotCharts, slicers and dashboard layout.

