<img width="209" height="82" alt="image" src="https://github.com/user-attachments/assets/bbcb8bf9-18e3-487a-8198-3bede366e576" />

## 🧭 Project Steps
1) Requirement Gathering / Business Requirements
2) Data Walkthrough
3) Data Connection (CSV → Power BI)
4) Data Cleaning / Quality Check (Power Query)
5) Data Modeling (star schema: FactSales + DimDate/DimOutlet/DimItem)
6) Data Processing (calculated columns, relationships)
7) DAX Calculations (KPIs & time intelligence)
8) Dashboard Layouting (grid, spacing, typography)
9) Charts Development & Formatting
10) Dashboard / Report Development
11) Insights Generation & Next Actions

## 🎯 Business Requirement
Goal: analyze Blinkit-style sales, customer satisfaction, and inventory distribution to find opportunities for optimization using KPIs and interactive visuals in Power BI.

**KPI Requirements**
- **Total Sales** – revenue from all items sold  
- **Average Sales** – average revenue per sale  
- **Number of Items** – total count of items sold  
- **Average Rating** – average customer rating

**Chart Requirements (what I built)**
1. **Total Sales by Fat Content** → Donut  
2. **Total Sales by Item Type** → Bar  
3. **Fat Content by Outlet (Total Sales)** → Stacked Column  
4. **Total Sales by Outlet Establishment (year)** → Line  
5. **Sales by Outlet Size** → Donut/Pie  
6. **Sales by Outlet Location (Tier)** → Bar/Funnel style card  
7. **All KPIs by Outlet Type** → Matrix (No. of items, Avg Rating, Avg Sales, Total Sales)

## 📈 Key Insights (sample from this dataset)
- **Tier-3** contributes the highest sales; **Medium** outlets lead (~$205K).
- **Top 3 item types ≈ ~60% of sales** → focus assortment & promos there.
- Avg rating holds around **~3.9**; consider quality initiatives for low-rated items.

> Numbers are from the sample dataset used in the `.pbix`; replace with your data as needed.

## 🧮 Core DAX (highlights)
- `Total Sales`, `Avg Sales`, `No of Items`, `Avg Rating`
- Time-intel: `Sales PY`, `YoY %`, `Sales PM`, `MoM %`
- Dynamic page `Title` reflecting slicers (Tier, Size, Item Type)
