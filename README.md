Dairy Analytics Power BI Dashboard
This Power BI report provides an end-to-end analysis of dairy farm operations, product shelf life, brand performance, and customer behavior across various dimensions such as location, storage condition, and channel. It leverages interactive visuals, DAX measures, and geographic insights to deliver a comprehensive dashboard.

📊 Key Business Questions Addressed
1. Performance of Dairy Farms Based on Location, Land Area, and Cow Population
Visual Type: Table

Columns:

Location

Sum of Land Area

Sum of Cow Population

Title: "Dairy Farm Performance by Region"

---

2. Brand-wise Sales Performance Across Regions
Visual Type: Matrix Table

Configuration:

Rows: Location

Columns: Brand

Values: Sum of Total Values

Purpose: Compare total brand sales across locations.

Title: "Brand Sales by Region"

---

3. Cow Population by Storage Condition
Visual Type: Stacked Bar Chart

Axes:

Y-axis: Storage Condition

X-axis: Sum of Cow Population

Title: "Cow Population by Storage Type"

4. Average Expiry Days by Product
Visual Type: Clustered Column Chart

Axes:

X-axis: Product Name

Y-axis: AvgExpiryDays (Calculated using DAX)

Measure Example:

DAX

AvgExpiryDays = AVERAGE(Products[ExpectedExpiryDays])
Title: "Average Expiry by Product"

---

5. Minimum and Maximum Shelf Life Products
Visual Type: Table or Card

Fields:

Product with Minimum Expiry Days

Product with Maximum Expiry Days

Purpose: Identify products with shortest and longest shelf life.

Title: "Shelf Life Range by Product"

---

6. Average Shelf Life by Storage Condition
Visual Type: Clustered Bar Chart

Axes:

Y-axis: Storage Condition

X-axis: AvgShelfLife (Calculated using DAX)

Measure Example:

DAX

AvgShelfLife = AVERAGE(Products[ExpectedExpiryDays])
Title: "Storage-wise Average Shelf Life"

---

7. Customer Purchase Behavior by Channel and Location
Visual Type: Pie Chart with Tooltip Page

Tooltip Page Name: "Sum of Quantity Sold by Location"

Tooltip Visual Type: Bar Chart

Y-axis: Location

X-axis: Sum of Quantity Sold

Purpose: Understand how purchase patterns vary across channels and regions.

Title: "Customer Purchase Distribution"

---

8. Geographic Distribution of Cow Population
Visual Type: Filled Map with Tooltip Page

Fields:

Location (Geography)

Cow Population

Tooltip Page Name: "Sum of Cow Population by Location"

Tooltip Visual Type: Bar Chart

Y-axis: Location

X-axis: Sum of Cow Population

Purpose: Visualize cow population across different geographic locations.

Title: "Cow Population Across Locations"

-------------------------------------------

🚀 Getting Started
Clone or download the repository.

Open Dairy_Analytics_Report.pbix in Power BI Desktop.

Use filters and tooltips to explore regional and categorical insights.

🛠 Tools & Techniques
Power BI Desktop

Data Modeling & Relationships

DAX for Calculated Columns and Measures

Tooltips & Filled Maps

Matrix and Chart Visualizations

📞 Contact
For queries or feedback:
YashMP550 – GitHub Profile
