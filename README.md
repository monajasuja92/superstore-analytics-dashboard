<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/c8dfc136-2e45-45f4-bbb1-30b50474fc02" />

👉 **[Click Here to Interact with the Live Tableau Dashboard](YOUR_TABLEAU_PUBLIC_OR_SERVER_LINK)**

---# Superstore Executive Analytics Dashboard FRD


# BUSINESS FUNCTIONAL REQUIREMENT DOCUMENT (FRD)

## 1. PROJECT CONTEXT & CONSTRAINTS
* **Business Problem**: Executives lack visibility into margin leakage, sub-category performance, and product return rates.
* **As-Is State**: Fragmented monthly Excel exports that delay decision-making and lack interactive drill-down capabilities.
* **Dependencies**: timely reverse-logistics logging for returns

---

## 2. DASHBOARD LAYOUT & DESIGN SYSTEM
* **Grid Framework**: Fixed 3-row structured hierarchy optimizing executive visual scanning from top to bottom.
* **Color Palette**: Light-gray canvas background (#F5F5F5) with bold accent coloring to isolate adjacent data blocks.
* **Visual Indicators**: Functional UI control shortcuts positioned in the top-right header for PPT, PDF, and Clear View.
* **Performance SLA**: All interactive filter changes and query rendering must compile completely in under 2 seconds.

---

## 3. GLOBAL FILTERS & CONTROLS
* **Metric Selector**: Radio-button container (Sales, Profit, #Orders) wrapped with a functional visual funnel icon.
* **Year Filter**: Dropdown menu allowing targeted chronological filtering of historical data.
* **Region Filter**: Multi-select dropdown initialized to (All) by default to scope data geographically.

---

## 4. EXECUTIVE SUMMARY (KPI CARDS)
* **TOTAL Sales**: Centered numeric display formatted in Indian Rupee notation showing total aggregated volume
* **PROFIT MARGIN**: Centered percentage calculated as (Sum of Profit / Sum of Sales) * 100, accurate to two decimals.
* **RETURN RATE**: Centered percentage calculated as (Count of Returned Orders / Count of Total Orders) * 100

---

## 5. REVENUE SEGMENTATION & ANALYTICAL CHARTS
* **Category By Sales**: Horizontal bar chart mapping parent categories with custom colors (Technology: Green, Furniture: Red, Office Supplies: Pink).
* **Sub-Category By Sales**: Sorted descending horizontal bar chart displaying explicit data value labels next to individual product lines.
* **Sales By States**: Filled geographic map visualization featuring dynamic overlay labels for State Name and Sales Value.
* **Top 5 Products**: Summary tabular grid hard-filtered to display only the top 5 records by the active metric selection.
* **Segment wise Sales**: Balanced donut chart showing customer segments (Consumer, Corporate, Home Office) with total volume inside the center.
* **Month Wise Sales**: Historical line graph tracked across continuous months, split by yearly grid lines, highlighting baseline and peak data points.
