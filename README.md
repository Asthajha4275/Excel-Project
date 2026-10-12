# Vrinda Store – Sales Data Analysis (Excel Dashboard)

An end-to-end Excel analysis of a year of online sales for **Vrinda Store**, an Indian ethnic-wear retailer selling across e-commerce marketplaces. The workbook cleans the raw order data, summarises it with PivotTables, visualises it in six charts, and combines everything into an interactive dashboard with slicers.

**Tools:** Microsoft Excel (data cleaning, PivotTables, PivotCharts, Slicers, Dashboard)

---

## 1. Business Problem

Vrinda Store wants to understand its 2022 sales performance in order to plan for the coming year. Key questions:

1. How do orders and revenue trend month by month?
2. Which gender and age group drives the most sales?
3. Which states and sales channels contribute the most revenue?
4. What share of orders is delivered vs. cancelled, returned or refunded?
5. Which product categories sell the most?

---

## 2. Dataset

| Item | Detail |
|---|---|
| Sheet | `Vrinda Store` |
| Size | 31,047 order lines × 21 columns |
| Period | January – December 2022 |
| Currency | INR |
| Total revenue | ₹21,176,377 |

**Key columns:** Order ID, Cust ID, Gender, Age, Age Group (Teenager / Adult / Senior), Date, Month, Status, Channel, SKU, Category, Size, Qty, Amount, ship-city, ship-state, ship-postal-code, B2B.

---

## 3. Project Steps

### Step 1 – Understand and import the data
- Loaded the raw order data into the `Vrinda Store` sheet.
- Reviewed each column, its data type and its meaning.

### Step 2 – Clean and prepare the data
- Checked for blank cells and duplicate rows (none remaining after cleaning).
- Standardised text columns (e.g. state names in upper case, category labels).
- Made sure `Date` is a proper date field and `Amount` is numeric.
- Created helper columns: **Month** (from Date) and **Age Group** (Teenager / Adult / Senior, from Age).
- Removed unused columns so the PivotTables stay light.

### Step 3 – Build PivotTables
One PivotTable per question, each on its own sheet:

| Sheet | Rows / Columns | Values |
|---|---|---|
| `chart 1 order vs sales` | Month | Sum of Amount, Count of Order ID |
| `chart2 men and women` | Gender | Sum of Amount |
| `chart 3 order status` | Status | Count of Order ID |
| `CHART 4 TOP 5 STATES` | ship-state (Top 5 filter) | Sum of Amount |
| `CHART 5 AGE GENDER` | Age Group × Gender | Count of Order ID (% of total) |
| `chart 6 channels` | Channel | Count of Order ID (% of total) |

### Step 4 – Create the charts
| # | Chart | Purpose |
|---|---|---|
| 1 | Combo / line chart – Orders vs Sales by month | Monthly trend |
| 2 | Pie chart – Men vs Women (sales) | Gender split |
| 3 | Bar chart – Order status | Fulfilment health |
| 4 | Bar chart – Top 5 states by sales | Geographic concentration |
| 5 | Chart – Age group by gender | Customer demographics |
| 6 | Pie chart – Sales channels | Channel mix |

### Step 5 – Build the interactive dashboard
- Placed all six charts on the `Dashboard` sheet with a consistent layout and colour theme.
- Added **three slicers – Month, Channel and Category** – connected to every PivotTable so the whole dashboard filters with one click.

### Step 6 – Draw insights and recommendations
See sections 4 and 5 below.

---

## 4. Key Insights

- **Revenue:** ₹21.18M across 31,047 order lines (about 28,471 unique orders), averaging roughly ₹682 per line.
- **Seasonality:** Sales peak in **March** (₹1.93M) and decline steadily through the year, with **November** the lowest (₹1.62M).
- **Gender:** **Women contribute ~64%** of revenue (₹13.56M) vs. ~36% from men (₹7.61M).
- **Age groups:** Adults are the largest segment for both genders (women ≈ 35%, men ≈ 15% of orders), followed by teenagers and seniors.
- **Top states:** Maharashtra (₹2.99M, ~14%), Karnataka (₹2.65M), Uttar Pradesh (₹2.10M), Telangana (₹1.71M) and Tamil Nadu (₹1.68M) together bring in about 48% of revenue.
- **Channels:** **Amazon** leads (~35% of revenue), then **Myntra** (~23%) and **Flipkart** (~22%). Together they account for roughly 80% of sales.
- **Order status:** ~92% of orders are delivered; the rest are returned (~3.4%), cancelled (~2.7%) or refunded (~1.7%).
- **Categories:** **Sets** generate about half of revenue (~50%), followed by kurtas (~23%) and western dresses (~15%).

---

## 5. Recommendations

1. **Target women aged 25–60** with campaigns, since they are the core buyers.
2. **Invest in Amazon, Myntra and Flipkart** (best returns), and test smaller channels such as Meesho and Ajio before scaling.
3. **Boost sales in the second half of the year** (Sep–Dec) through festive offers, as sales dip steadily after March.
4. **Expand in Maharashtra, Karnataka, Uttar Pradesh, Telangana and Tamil Nadu**, and run marketing tests in under-served states.
5. **Focus on Sets and kurtas** for inventory planning.
6. **Reduce returns and cancellations** (~8% of orders) with better size guides and product descriptions.

---

## 6. How to Use the Workbook

1. Download `Vrinda_store_data_Analysis_project_1.xlsx` and open it in Microsoft Excel (desktop version recommended for slicers).
2. Go to the **Dashboard** sheet.
3. Click any value in the **Month**, **Channel** or **Category** slicers to filter all charts together (hold Ctrl for multiple selections; use the funnel icon to clear).
4. Explore the individual pivot sheets to see the numbers behind each chart.

---

## 7. Repository Structure

```
├── Vrinda_store_data_Analysis_project_1.xlsx   # Data, PivotTables, charts, dashboard
└── README.md
```

## 8. Skills Demonstrated

Data cleaning · PivotTables & PivotCharts · Slicers · Dashboard design · Business insight generation

---

**Author:** Astha Kumari Jha
**GitHub:** [github.com/Asthajha4275](https://github.com/Asthajha4275)# Excel-Project_ VRINDA STORE DATA ANALYSIS.
DASHBOARD:

