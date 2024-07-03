# Sales Performance Dashboard

## Overview
This project involves creating a Sales Performance Dashboard using Microsoft Power BI to help executives understand overall sales performance, identify trends, and make informed decisions about sales strategies.

## Data Source
The dataset used for this project is the "Superstore Sales Dataset" from Kaggle. It contains monthly sales data, product categories, sales regions, and sales representatives.

## Steps to Replicate
### Phase 1: Load Data
1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/juhi1994/superstore-sales).
2. Load the dataset into Power BI.

### Phase 2: Data Cleaning
1. Open Power Query Editor by clicking "Transform Data".
2. Enable "Column Quality" and "Column Distribution" from the "View" tab.
3. Handle missing values:
   - Remove rows with significant missing data by right-clicking the column and choosing "Remove Empty".
   - Fill missing values using "Fill Down" or "Fill Up".
4. Change data types as necessary:
   - Ensure dates are set to Date type.
   - Ensure numerical columns are set to Decimal Number type.
5. Remove unnecessary columns.
6. Create calculated columns if needed.

### Phase 3: Create Calculated Columns
1. **Sales per Unit**:
   - In Power BI Desktop, go to the Data view.
   - Click on the table name in the Fields pane.
   - Click on "New Column" in the Modeling tab.
   - Enter the formula: `Sales per Unit = DIVIDE([Sales], [Quantity])`.
2. **Order Year**:
   - In Power BI Desktop, go to the Data view.
   - Click on "New Column" in the Modeling tab.
   - Enter the formula: `Order Year = YEAR([Order Date])`.
3. **Order Month**:
   - In Power BI Desktop, go to the Data view.
   - Click on "New Column" in the Modeling tab.
   - Enter the formula: `Order Month = FORMAT([Order Date], "MMMM")`.

### Phase 4: Data Modeling
1. Create relationships between tables if multiple tables are used.

### Phase 5: Create Visualizations
1. **Total Sales:** Use a Card visualization.
2. **Sales by Region:** Use a Bar Chart.
3. **Top Performing Products:** Use a Column Chart.
4. **Sales Trend:** Use a Line Chart.
5. **Sales by Representative:** Use a Bar Chart.
6. **Profit Margin Analysis:** Use a Gauge Chart.

### Phase 6: Design the Dashboard
1. Arrange visualizations logically.
2. Add titles, labels, and legends.
3. Apply filters and slicers for interactivity.
4. Use formatting features for better visual appeal.

### Phase 7: Export and Publish
1. Export the report to PDF for sharing.
2. Save the report as a .pbix file.
3. Create a GitHub repository and upload the .pbix file and README.md.

## Summary Statistics Analysis

### Key Findings

1. **Total Sales:**
   - Each region (South, West, Central, and East) has the same total sales amounting to 2,261,536.7827. This indicates that the sales distribution across regions is uniform, which might be due to data duplication or an issue in the calculation.

2. **Average Sales:**
   - The average sales per order for all regions are consistent at 230.77. This uniformity suggests that the average sales per transaction do not vary significantly across regions.

3. **Minimum Sales:**
   - The minimum sales amount recorded is 0.444 across all regions. This shows that there are very low-value sales transactions occurring in all regions.

4. **Maximum Sales:**
   - The maximum sales amount recorded is 22,638.48 across all regions. This indicates that there are high-value sales transactions occurring uniformly in all regions.

5. **Total Orders:**
   - The total number of orders for each region is 9,800. This further confirms the uniformity across regions, suggesting potential data issues.

### Interpretation

- The uniformity in the summary statistics across all regions raises questions about the data's accuracy. Normally, we would expect some variation in total sales, average sales, minimum sales, maximum sales, and the number of orders across different regions.
- It is essential to re-evaluate the data extraction and calculation process to ensure there are no errors or duplications.
- If the data is accurate and such uniformity is real, it might indicate a highly balanced sales distribution strategy across regions, ensuring equal sales opportunities and performances.

## Dashboard Screenshots

https://github.com/Kelechiede/SalesPerformanceDashboard.git
### Central Region
![Central Region Dashboard](Github-PowerBI_Tableau/sales_performance_central.png)

### East Region
![East Region Dashboard](Github-PowerBI_Tableau/sales_performance_east.png)

### West Region
![West Region Dashboard](Github-PowerBI_Tableau/sales_performance_west.png)

### South Region
![South Region Dashboard](Github-PowerBI_Tableau/sales_performance_south.png)

## Files
- SalesPerformanceDashboard.pbix
- README.md

## License
This project is licensed under the MIT License.
