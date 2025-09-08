
# FINANCIAL ANALYSIS PROJECT

## PROJECT DESCRIPTION
   This project aims to provide actionable insights into the financial performance of a business by analyzing revenue data across multiple dimensions,
   including subcategories, branches and payment methods.
   The project delivers interactive dashboard and reports to help stakeholders identify revenue drivers, assess trends and inform strategic decisions 
   such as resource allocation,marketing strategies and operational improvements.

### SOFTWARE USED
    * EXCEL
    * POWER BI

### STEPS FOLLOWED
    * Step 1: Load data into power bi desktop, dataset is an xlsx file.
    * Step 2: Open power query editor to check for duplicates, empty cells and missing values.
    * Step 3: Remove duplicates, empty cells and fill up missing values using the fill up & down option (fill with average).
    * Step 4: Click on the close&apply button on the menu bar to close the power query editor window and apply any pending changes.

### ADD CALCULATED TABLE
    * Step 5: Using the Date column from the dataset to create a date table
               . DATE TABLE = CALENDARAUTO()

    * Step 6: Extracting the month and day from the Date Table
               - MONTH = FORMAT('DATE TABLE'[Date],"MMMM")
               - DAY = FORMAT('DATE TABLE'[Date],"DDDD")

### USE DAX (DATA ANALYSIS EXPRESSION) TO CREATE MEASURES FOR KEY METRICS, SUCH AS:
    * Step 7: TOTAL TRANSACTION = COUNT(Sheet1[Transaction ID])

    * Step 8: TOTAL AMOUNT = SUM(Sheet1[Amount])

    * Step 9: AVERAGE REVENUE = AVERAGE(Sheet1[Amount])

    * Step 10: TOTAL REVENUE = CALCULATE(COUNT(Sheet1[Revenue or Expense]),'Sheet1'[Revenue or Expense]="REVENUE")

    * Step 11: TOTAL EXPENSE = CALCULATE(COUNT(Sheet1[Revenue or Expense]),'Sheet1'[Revenue or Expense]="EXPENSE")

### VISUALIZATIONS
    * Step 12: Revenue by sub-category <Stacked Bar Chart>
                This chart describes how revenue is broken down by sub-categories in the dataset. It helps to identify key revenue drivers, access
                performance trends and support strategic financial decisions.

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/3f94e031-88f1-4b19-9e39-f14caeba884b" />

    * Step 13: Correlation between Payment Method <Donut Chart>
                It explores how payment methods(e.g card, mobile phone, transfer, cash) correlate with financial metrics like revenue, transaction
                volume in the dataset aiding in optimizing payment strategies and financial planning. 
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/93993fc1-ec7b-421f-be71-41a747f8a47e" />

    * Step 14: Revenue trends by month <Line Chart>
                This chart explains how to analyze monthly revenue trends to identify seasonality, growth patterns and anomalies. It helps stakeholders
                plan budgets, forecast performance and optimize strategies for product/service segment.
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/f650f00f-d825-4b88-880a-f75cef75b74c" />

    * Step 15: Branch vs sub-category <Matrix>
                It clarifies the difference between branch and sub-category and how they are used to analyze revenue, comparing these dimensions helps
                identify which location or product drive revenue.
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/c549b931-eb5b-4a0d-aa49-d545e2e8f3da" />

    * Step 16: Revenue by sub-category <Tree Map>
                This explains how revenue is distributed across subcategories (are specific product or service segments). This analysis helps identify
                key revenue drivers and inform strategic financial decisions.
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/7278552c-54d0-4ed7-85f0-2e3799f5f391" />

    * Step 17: Revenue by branch <Stacked Bar Chart>
                This chart explains how revenue is distributed across branches. It helps to identify high-performing locations and supports decisions 
                on staffing, operations or regional strategies.
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/502341c4-598d-417f-a927-55dd7dfe7aa7" />

### ADD INTERACTIVITY WITH SLICERS
    1. Select the slicer visual: In the visualizations pane (on the right), click the slicer icon. This adds a blank slicer to your report canvas.
    2. Add a field to the slicer: In the fields pane, locate the dataset and drag the field you want to filter (Year and Branch) into the 
       or values area of the slicer.
    3. Resize and format the slicers to control user interactions.

### CONCLUSION
    This dashboard visualizes key financial metrics focusing on monthly revenue trends,profitability, identifying high-performing locations
    and key revenue drivers. Built for analyst and investors, it supports strategic decision-making by highlighting growth patterns and risks.
    The visualizations and underlying data are accessible via the 
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/474a02c3-aac0-4019-a5db-09bf718de651" />
