# Global Sales Performance Dashboard

# 1. Project Overview

**Key business questions**
- What does the current business landscape look like?
- How are the individual markets performing?
- How are the individual product groups performing?

**Data model (Star Schema)**

| Type | Tables |
|---|---|
| Fact | `factOrder`, `Return` |
| Dimension | `dimDate`, `dimProduct`, `dimRegion`, `dimCustomer`, `People` |
| Supporting | `_Measures`, `Parameters` (Metric Selector) |

**Key measures:** Total Sales, Total Orders, Total Profit, Profit Margin, Average Order Value (AOV), Quantity Sold, Return Rate, Sales/Profit/AOV Growth, YoY Growth.

---

## 2. Dashboard Structure

| Page | Content |
|---|---|
| **Executive Summary** | Overall KPIs and % change, Sales & Profit trends over time, performance by Sub-Category and Market, Segment breakdown, Top Sales Persons, Top Customers |
| **Market Performance Analysis** | Best region, highest profit/margin/YoY growth markets, Sales vs. Profit Margin scatter (Scale up / Cash cow / Invest / Reconsider), Return Rate by market, Decomposition Tree, detail table by Market → City |
| **Product Performance Analysis** | Top categories by Sales/Orders/Profit/Margin, lowest Return Rate, Sales Growth treemap, Sales vs. Margin scatter by Sub-Category, detail table by Category → Product |
| **Insights and Recommendations** | Summary of insights and recommendations for Markets, Products and overall strategy |

---

## 3. Main visualizations
- Executive Summary
  - Main KPIs <img width="1026" height="86" alt="image" src="https://github.com/user-attachments/assets/d076fda7-4f6f-4dc9-8a54-9b3d8d9fb059" />
  - Sales metrics by Time and Market <img width="1018" height="574" alt="image" src="https://github.com/user-attachments/assets/256785b6-4505-4897-8be1-72ac28272e59" />
  - What / Who contributes most to Total Sales? <img width="1271" height="690" alt="image" src="https://github.com/user-attachments/assets/fce6b6f1-3e4d-431d-8dc3-bb84d11cfe61" />

- Market performance
  - Trend and breakdown of key Metrics <img width="1279" height="621" alt="image" src="https://github.com/user-attachments/assets/c0859ef8-ebe7-4ae6-bd5b-836f682fa75c" />
  - Market categories based on key Metrics <img width="1010" height="564" alt="image" src="https://github.com/user-attachments/assets/bd998b37-6190-496a-8be1-c19702adbb9f" />

- Product performance
  - Trend and breakdown of key Metrics <img width="756" height="678" alt="image" src="https://github.com/user-attachments/assets/dc55ded4-510d-4932-ad21-a91a08ba23c7" />
  - Product categories based on key Metrics <img width="674" height="274" alt="image" src="https://github.com/user-attachments/assets/428aae90-bd30-49c4-b383-fee88d649c6e" />


---

## 4. Main Findings

### Overall
- The company is growing well: **Sales ~26% per year**, **Profit ~24% per year**, and **Profit Margin steady above 11%**.
- **APAC, EU and US** are the three main revenue drivers, consistently ranking in the top 3 for Sales, Profit and Profit Margin. Growth has slowed, most likely because these markets are maturing rather than declining.

### Markets
- **APAC** has the highest sales (**~$3.6M**) but low Profit Margin and AOV, especially **Southeast Asia (PM only ~2.02%)**.
- **EU, US, Oceania and Central Asia** deliver strong profit (average PM **~13.5%**) and sustainable growth (**~24.22%**).
- **China, Japan, Hong Kong, the UK, Finland and Norway** have high margins (average **~22.7%**) but a **high Return Rate (~13.31%)** and low RCR, particularly Japan and the UK (~3%).
- **Canada, South Africa and the Middle East** currently contribute little (~$175.83K) but show **very strong sales growth (~70.28%)**, indicating significant untapped potential.

### Products
- **Technology** is the strongest category, leading in Sales, Profit and Profit Margin.
- **Full-size Smartphones** have the highest sales, healthy margins (**6.81% – 23.27%**) and double-digit growth (**27.5% – 67.81%**), with the exception of Nokia.
- **Machines** have low margin (**7.56%**) and low growth (**17.48%**). Some Copier/Machine products have high sales but are slowing down or showing negative growth.
- **Furniture** is generally less effective. **Tables** are the weakest, with many products showing negative margin, negative growth and a Return Rate of **7.54%**. In contrast, Bookcases, Adjustable Leather Chairs and Furnishings perform better (5 Adjustable Leather Chair products account for **~50% of Furniture sales**, with growth of **25.47%**).
- **Office Supplies** have healthy margins despite lower sales. Paper and Envelopes have high margins, while a few Storage products are loss-making (Hoover Stove White, Hamilton Beach Stove Silver).
- **Accessories** have a relatively high Return Rate. The most frequently returned groups are Fasteners, Accessories, Appliances and Furnishings.

---

## 5. Main Recommendations

### Markets
1. **Maintain investment in APAC, EU and US, and improve profitability in Southeast Asia.** Shift the product mix toward high-margin products and roll out bundle packages in Indonesia, the Philippines, Thailand and Vietnam.
2. **Reduce return rates before expanding in North Asia and some European markets.** Review the reasons for returns, tighten quality control on frequently returned products, and improve after-sales service.
3. **Expand selectively into emerging markets (Canada, South Africa, the Middle East).** Add distribution partners and localized marketing, while closely monitoring profitability before scaling up.

### Products
1. **Prioritize the premium smartphone category** (increase inventory and promotions for Full-size Smartphones). Review costs for Canon Advanced Copiers and underperforming Machines products.
2. **Reallocate resources from Tables to higher-margin Furniture products.** Reduce Tables inventory and promotional spending.
3. **Optimize the Office Supplies product mix.** Review loss-making Storage products, and push Paper, Envelopes and certain profitable Appliances.

### Overall Strategy
- **Prioritize profit quality over revenue scale:** optimize pricing, limit excessive discounting, and push high-margin categories in markets with high sales but low margins.
- **Analyze Return Rate at the SKU level**, especially for Accessories, combined with improvements in quality, product information and after-sales support.
- **Diversify revenue** by gradually expanding the distribution network in Canada and EMEA.
- **Rebalance Furniture:** shift inventory, marketing and promotions toward products with sustainable margin and growth, while reviewing pricing and costs for underperforming groups.
