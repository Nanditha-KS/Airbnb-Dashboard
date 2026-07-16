# Airbnb Listings Analysis — Chicago vs New Orleans

## 📊 Project Overview
This project analyzes Airbnb listings data from Chicago and New Orleans to uncover insights around pricing, room types, host behavior, and listing availability. The workflow covers the full data analytics pipeline — from raw data cleaning in Python to an interactive multi-dashboard visualization built in Tableau.

## 🔗 Live Dashboard
👉 [View the interactive Tableau dashboard here](YOUR_TABLEAU_PUBLIC_LINK_HERE)

## 🛠️ Tools Used
- **Python (Pandas, NumPy)** — Data cleaning and transformation, done in Google Colab
- **Tableau Public** — Interactive dashboard design and data visualization

## 📁 Repository Contents
| File | Description |
|---|---|
| `Aiebnb.ipynb` | Google Colab notebook containing the full data cleaning and feature engineering process |
| `airbnb_clean.csv` | Final cleaned dataset used for the Tableau dashboards |
| `Chikago.csv` / `Neworleans.csv` | Original raw datasets (Chicago and New Orleans Airbnb listings) |
| `/screenshots` | Preview images of each dashboard |

## 🧹 Data Cleaning Summary
- Combined two city datasets (Chicago: 8,660 rows, New Orleans: 7,189 rows) into a single unified dataset with a `city` label column.
- Trimmed down from dozens of raw columns to 16 essential fields.
- Cleaned the `price` column (removed currency symbols, converted to numeric, filtered outliers > $2,000).
- Filled missing values in `reviews_per_month`, `last_review`, `neighbourhood`, and `neighbourhood_group`.
- Removed duplicate listings based on unique ID.
- Standardized neighbourhood name formatting.
- Engineered 4 new analytical columns:
  - `price_category` (Budget → Luxury)
  - `availability_category` (Low → Always Available)
  - `review_activity` (No Reviews → Highly Active)
  - `host_type` (Casual, Growing, Professional — based on number of listings per host)
- Final cleaned dataset: **13,944 rows × 23 columns**

## 📈 Dashboard Highlights
- **Dashboard 1 — Overview:** City-level KPIs, listings map, and listing counts by city.
- **Dashboard 2 — Room Type & Pricing:** Room type distribution, price comparisons across room categories.
- **Dashboard 3 — Price & Review Trends:** Price distribution histogram, price vs. reviews scatter analysis.
- **Dashboard 4 — Host Insights:** Host type distribution, average price and review activity by host type.

## 🖼️ Preview
![Dashboard Screenshot](screenshots/dashboard1.png)

## 👤 Author
**Nanditha K S**
