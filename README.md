# 📊 Sales and Refund Dashboard (2025)

An interactive **Power BI** dashboard that analyses a full year of e-commerce orders and returns to show where refunds come from, why customers send products back, and how returns affect revenue.

> **Period covered:** 1 Jan 2025 – 31 Dec 2025
> **Tool:** Power BI Desktop (2 report pages)

---

## 🎯 Objective

Answer four business questions:

1. How large is the return problem (rate and refund cost)?
2. Which categories, sub-categories and products drive returns?
3. Why are customers returning items?
4. How do returns move with revenue across the year and across sales channels?

---

## 🖼️ Dashboard Preview

<!-- Replace with your own screenshots, e.g. upload to /images and link below -->
| Page 1: Overview | Page 2: Deep Dive |
|---|---|
| ![Overview](images/page1_overview.png) | ![Deep dive](images/page2_deep_dive.png) |

---

## 🧭 Report Pages

### Page 1: Overview
- KPI cards: Total Order, Return Order, Return Unit, Return Rate, Refund Amount, Avg Return Days
- Net Revenue by Month (area chart)
- Total Order by Sales Channel (pie chart)
- Return Order by Category (bar chart)
- Slicers: Date range, Month, Sales Channel, Customer State, Return Reason

### Page 2: Deep Dive
- Refund Amount and Return Order by Month (column + line combo)
- Total Order and Return Order by Category (clustered bar)
- Product-level table: Total Order, Return Order, Return Units, Return Rate, Refund Amount, Avg Return Days
- Return Units by Sales Channel (donut chart)
- Sub-category × Return Reason heatmap (matrix)

---

## 📈 Key Metrics

| Metric | Value |
|---|---|
| Total orders | 4,286 |
| Return orders | 792 |
| Return units | 1.14K |
| **Return rate** | **18.48%** |
| **Refund amount** | **3.82M** |
| Average return days | 14.88 |

---

## 🔍 Key Findings

1. **Return rate is high.** Almost 1 in 5 orders is returned (18.48%), costing 3.82M in refunds.
2. **Returns peak with sales in Q4.** Net revenue grows from 1.34M (Jan) to 2.54M (Dec). Monthly return orders sit at about 46–59 for Jan–Sep, then climb to 78 (Oct), 97 (Nov) and 137 (Dec), with refunds reaching roughly 500K in December.
3. **Fashion and Electronics lead returns.**

   | Category | Return orders |
   |---|---|
   | Fashion | 280 |
   | Electronics | 201 |
   | Home & Kitchen | 123 |
   | Sports | 70 |
   | Beauty | 69 |
   | Books | 49 |

   Fashion and Electronics together account for about 60% of the 792 returns.
4. **Channel mix.** Orders: Website 33.43%, Mobile app 31.47%, Marketplace 25.57%, Offline store 9.52%. Return units follow a similar split, so no channel is a clear outlier.
5. **Return reasons are product-specific.**
   - *Wrong size:* Men's Clothing (56), Footwear (44), Women's Clothing (37)
   - *Damaged product:* Kitchen (26), Mobile Accessories (21)
   - *Defective product:* Smart Devices (27), Audio (19), Mobile Accessories (20)
6. **One product stands out.** NorthLane Slim Fit Jeans: 22 returns on 62 orders, a **35%** return rate, almost double the overall average.

---

## 💡 Recommendations

- Add size guides, fit reviews and "true to size" ratings for apparel and footwear.
- Review packaging and carrier handling for kitchen items and mobile accessories.
- Run supplier quality checks on Smart Devices and Audio.
- Investigate NorthLane Slim Fit Jeans (sizing, product description or quality).
- Plan Q4 for higher return volume: extra staffing, clear return-policy messaging, stock buffers.
- Standardise return-reason labels at source (see Data Notes).

---

## 🗂️ Data Notes

- Return reasons contain near-duplicate labels (e.g. "Not As Expected" vs "product not as expected", "defective product" vs "Damaged Product"), which splits counts. Merge them in Power Query for cleaner reason analysis.
- Return rate = Return Orders ÷ Total Orders (792 ÷ 4,286 = 18.48%).

<!-- Add details about your dataset: source, number of rows, tables, and columns -->

---

## 🛠️ Tech Stack

- Power BI Desktop
- DAX (measures such as Return Rate, Refund Amount, Avg Return Days)
- Power Query (data cleaning and transformation)

---

## 🚀 How to Use

1. Clone or download this repository.
2. Open `Sales_and_Refund_Dashboard.pbix` in Power BI Desktop.
3. Use the slicers (date, month, channel, state, return reason) to explore the data.

<!-- Rename the .pbix file above to match yours -->

---

## 🔭 Future Improvements

- Clean and merge return-reason labels
- Fix chart title typo ("Net Revenue by Month")
- Add a key-takeaway text box on each page
- Simplify heatmap colours with a legend
- Add a forecast for Q4 return volume

---

## 👤 Author

**Your Name**
[LinkedIn](https://www.linkedin.com/) · [Portfolio](#) · [Email](mailto:you@example.com)

⭐ If you found this project useful, consider giving the repo a star.
