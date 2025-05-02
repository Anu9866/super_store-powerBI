# super_store-powerBI
# 📊 Sales Dashboard – Superstore Data (Power BI)

This project presents an interactive **Sales Dashboard** built using **Power BI**. It provides key insights into sales performance by **product segment**, **region**, and **month** using visuals and filters.

---

## 🛠 Tools Used

- Power BI Desktop
- Superstore_Sales.csv dataset (or similar structure)
- (Optional) Python + Pandas for data cleaning

---

## 📁 Dataset Overview

The dataset includes the following columns (minimum required):

- `Order Date` – Date of each sale
- `Region` – Sales region (e.g., West, East)
- `Segment` – Customer segment (e.g., Consumer, Corporate)
- `Sales` – Sales amount in USD
- `Profit` – Profit amount in USD

If `Category` is missing, `Segment` or `Sub-Category` is used as an alternative in the donut chart.

---

## 📊 Dashboard Components

The Power BI dashboard contains the following visuals:

1. **Line Chart** – Monthly Sales Trend (`Order Date` in "MMM YYYY" format)
2. **Bar Chart** – Sales by Region
3. **Donut Chart** – Sales by Segment (or Sub-Category)
4. **Slicer** – Interactive filter for Region

All visuals use color emphasis to highlight top-performing areas.

---

## 🚀 How to Use

1. Open `Power BI Desktop`
2. Import the dataset (`Superstore_Sales.csv`)
3. Create a new column for Month-Year:
   ```DAX
   MonthYear = FORMAT('Table'[Order Date], "MMM YYYY")
