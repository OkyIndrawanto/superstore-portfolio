
---

## Dataset details

**Source:** Tableau’s "Sample - Superstore" dataset (publicly available)  
**Rows:** ~10k  
**Key columns after cleaning:**
- `row_id`, `order_id`, `order_date`, `ship_date`, `ship_mode`
- `customer_id`, `customer_name`, `segment`
- `city`, `state`, `postal_code`, `region`
- `product_id`, `category`, `sub_category`, `product_name`
- `sales`, `quantity`, `discount`, `profit`

**Cleaned CSV:** sql/superstore_dataset.superstore_clean.csv
Includes standardized `snake_case` column names for SQL & BI tool compatibility.

---

## Tools & skills used
- **Google BigQuery** — data cleaning, transformation, analysis
- **SQL** — aggregations, filtering, date functions, calculated fields
- **Tableau Public** — dashboard design, interactivity (filters, highlights)
- **Data storytelling** — summarizing complex findings into clear visuals

---

## SQL scripts
1. `create_superstore_clean.sql` — clean & rename columns  
2. `01_top_product_categories.sql` — total sales by category  
3. `02_top_customers.sql` — top 10 customers by sales  
4. `03_yearly_trend.sql` — yearly sales & profit trend  
5. `04_top_states_profit.sql` — top states by profit  
6. `05_shipping_delivery.sql` — average delivery time by ship mode

---

## Key insights from the dashboard
- **High concentration of sales** in a few categories → potential inventory focus areas.
- **Top 10 customers** generate significant revenue — retention opportunity.
- **Yearly trend** shows seasonal peaks — useful for demand planning.
- **Profitability varies by state** — could guide targeted marketing.
- **Shipping speed differences** highlight operational improvement areas.

---

## Tableau Dashboard
**Interactive Link:** [Open in Tableau Public](https://public.tableau.com/shared/NPN8XRTGB?:display_count=n&:origin=viz_share_link)  

**Features:**
- Filters for **Region**, **Category**, and **Year**
- Consistent color palette for readability
- Currency formatting with `$` for sales metrics
- KPI cards, bar charts, and line trends for a comprehensive overview

---

## How to reproduce
1. Upload `superstore_dataset.superstore_clean.csv` to BigQuery (see SQL DDL in `/sql`).
2. Run the five SQL files in `/sql` on the table `your_project.your_dataset.superstore`.
3. Upload data to Tableau and rebuild the visualizations using the worksheets in `/tableau`.
4. Export dashboards to images for documentation.


---

## Contact
Created by: **[Oky Indrawanto]** — data analyst portfolio  

