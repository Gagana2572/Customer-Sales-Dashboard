# Customer & Sales Dashboard

An interactive **Tableau** report that analyzes 2023 sales performance and customer behavior, with year-over-year comparisons against 2022.

🔗 **[View the live dashboard on Tableau Public](https://public.tableau.com/views/Book1_17897692925930/SalesDashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**

---

## Overview

This project contains two linked dashboards that answer two core business questions:

1. **Sales Dashboard**: How are sales, profit, and quantity trending, and which product subcategories drive (or drag down) results?
2. **Customer Dashboard**: How many customers do we have, how often do they order, and who are our most profitable customers?

Both dashboards share the same layout and navigation (icons in the header switch between views, and a filter control sits alongside), and use a consistent color scheme: **blue** for highest month / profit / above average, **orange** for lowest month / loss / below average.

---

## Sales Dashboard

<p align="center">
  <img src="images/sales_dashboard.png" alt="Sales Dashboard" width="900">
</p>

### KPI Cards (2023 vs. 2022)

| Metric | 2023 Value | Change vs. Prior Year |
|---|---|---|
| Total Sales | $733K | ▲ 20.4% |
| Total Profit | $93K | ▲ 14.2% |
| Total Quantity | 12K | ▲ 3.2% |

Each card includes a sparkline comparing 2023 (dark line) against 2022 (gray line) from January to December, with markers for the **highest** (blue) and **lowest** (orange) months.

### Sales & Profit by Subcategory

- Compares 2023 sales against 2022 sales for each subcategory (dark bar = 2023, light bar = 2022).
- A paired profit chart shows profit (blue) or loss (orange) per subcategory.
- Orange dots flag the lowest-performing subcategories (e.g., Machines, Envelopes, Fasteners).
- Phones, Chairs, and Binders lead in sales; Tables and Machines show negative profit.

### Sales & Profit Trends over Time

- Weekly step-line charts for sales and profit across the year.
- Reference lines show the weekly averages (**≈ $14K sales**, **≈ $2K profit**).
- Segments are colored **blue** when above average and **orange** when below.

---

## Customer Dashboard

<p align="center">
  <img src="images/customer_dashboard.png" alt="Customer Dashboard" width="900">
</p>

### KPI Cards (2023 vs. 2022)

| Metric | 2023 Value | Change vs. Prior Year |
|---|---|---|
| Total Customers | 793 | ▲ 8.6% |
| Total Sales Per Customer | 1,058 | ▲ 10.8% |
| Total Orders | 1,687 | ▲ 28.3% |

### Customer Distribution by Number of Orders

A bar chart showing how many customers placed 1, 2, 3 … 8 orders in 2023. Most customers fall in the 1–3 order range (200, 200, and 156 customers respectively), with a long tail of repeat buyers.

### Top 10 Customers by Profit

A ranked table with each customer's last order date, 2023 profit, 2023 sales, and number of orders.

| Rank | Customer | 2023 Profit | 2023 Sales | Orders |
|---|---|---|---|---|
| 1 | Raymond Buch | $6,781 | $14,203 | 3 |
| 2 | Hunter Lopez | $5,046 | $10,523 | 2 |
| 3 | Tom Ashbrook | $4,599 | $13,723 | 2 |
| 4 | Andy Reiter | $2,608 | $5,821 | 2 |
| 5 | Jane Waco | $1,953 | $5,385 | 4 |
| 6 | Helen Wasserman | $1,947 | $8,166 | 5 |
| 7 | Brian Moss | $1,938 | $5,683 | 5 |
| 8 | Alan Dominguez | $1,867 | $5,434 | 4 |
| 9 | Jim Epp | $1,704 | $4,074 | 4 |
| 10 | Steven Roelle | $1,676 | $3,506 | 1 |

---

## Key Takeaways

- **Growth across the board:** sales (+20.4%), profit (+14.2%), and quantity (+3.2%) all increased year over year.
- **Orders grew faster than customers:** orders rose 28.3% while the customer base grew 8.6%, suggesting stronger repeat purchasing.
- **Profit is not evenly distributed:** some subcategories (Tables, Machines) generate losses despite meaningful sales and deserve a pricing or discount review.
- **A few customers matter a lot:** the top 3 customers alone contribute over $16K in profit, and the #1 customer placed only 3 orders, so order size, not frequency, drives top-customer value.

---

## Skills & Tools

| Skill / Tool | Application in This Project |
|---|---|
| **SQL** | Querying and aggregating the data: joins across orders, customers, and products; sales, profit, and quantity metrics; year-over-year comparisons; customer order counts and rankings |
| **Tableau** | Building the interactive dashboards: KPI cards with sparklines, diverging profit/loss bars, reference lines with above/below-average coloring, ranked tables, and dashboard navigation and layout |

---

## Data

The dashboards are built on a retail sales dataset (orders, customers, products, sales, profit, and quantity) covering 2022–2023. *(Add your data source and a link here, e.g., the Superstore sample dataset, if applicable.)*
