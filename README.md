# Data Cleaning with Power Query - Unpivoting Messy Data

## 📋 Project Overview
Transformed a messy, wide report into a clean, tidy table using Excel + Power Query.

## 😖 Before - Dirty 3 (The Problem)
- Ship Mode (First Class, Same Day, Second Class) was on top row
- Segment (Consumer, Corporate, Home Office) was on second row
- Sales scattered across many columns with lots of blank cells
- Impossible to filter or analyse

## 🧹 Step 1 - Fixed Headers in Excel (Before Power Query)
1. Created another row for header in the Excel sheet
2. Renamed all columns manually, combining Ship Mode + Segment:
   - First Class - Consumer
   - First Class - Corporate
   - First Class - Home Office
   - Same Day - Consumer, etc.
3. Deleted the old messy 2 header rows (Ship Mode row + Segment row)
Now each Sales column had one clear name.

## 🧹 Step 2 - Deep Cleaning in Power Query
1. Loaded the fixed sheet into Power Query
2. Unpivoted Columns - turned all the wide Sales columns into 2 columns: Ship Mode / Segment + Sales
3. Split Ship Mode / Segment back into 2 separate columns
4. Removed blank rows and errors
5. Fixed Order Date to proper Date format
6. Fixed Sales to Number/Currency
7. Renamed columns cleanly and loaded as cleanedbyPowerQuery

## ✨ After - cleanedbyPowerQuery (The Result)
Clean tidy table with only 5 columns:
Order ID | Order Date | Ship Mode | Segment | Sales

Example:
CA-2011-103366 | 01-15-2013 | First Class | Consumer | 149.95

Every row = One Order. No blanks.

## 🛠️ Tools Used
- Microsoft Excel
- Power Query Editor

## 📊 Why It Matters
Before = Report to look at. After = Data to analyse.
Now ready for Pivot Tables, Charts and Dashboards.

---
*Created by Mariam44*
