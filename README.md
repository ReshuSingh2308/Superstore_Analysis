# Superstore_Analysis

## Project Description
Cleaning Superstore sales data with Excel and Visualizing it with the help  of Power Bi.

## Steps Performed
1. Handled missing values
2. Fixed misaligned columns
3. Fixed the date columns(Text to Date format(dd-mm-yyyy)) of Order_Date and Shipment_Date.

## Files Included
- `data/raw/Superstore.csv`: Original data
- `data/processed/Superstore_dashboard.xlsx`: Cleaned data
- `docs/cleaning_steps.md`: Detailed steps

## Tasks Performed In Excel
1.Download the dataset from Kaggle.

2.Imported the dataset to Excel.

3.Checked the dataset for any dublicate datas.
  By using the data tools in data option.
  
4.Checked the columns for extra spaces and Standerdizing the names/title of the movies ot tv-series.
  For Removing extra spaces Formula(=TRIM(INDEX PLACE)).
  For standersizing the text Formula(=PROPER(INDEX PLACE)).

5. Converted the Order_Date  and ship_date into DateTime format. 
    Formula used{=IF(ISNUMBER(A2), A2, IFERROR(DATE(VALUE(RIGHT(A2, 4)), VALUE(MID(A2, FIND("/", A2) + 1, FIND("/", A2, FIND("/", A2) + 1) - FIND("/", A2) - 1)), VALUE(LEFT(A2, FIND("/", A2) - 1))), ""))}

## Tasks Performed In Power BI

1.Imported the csv file in Power Bi.

2.Made a visualization on the the Top 10 States of United States which has placed the most number of orders from Superstore.
  Used Clustered Bar Graph for it.
  
3.Top 5 Cities of United States which has placed the most number of orders from Superstore.
  Used Pie Chart for it.

4.Made a Pie Chart about which categories of product has the higher percentage of sales.
  Used Pie Chart for it.

5.Used 3 Cards :-
 i. For Total Sales.
 ii.For Total Profit.
 iii. For Total Quantity Ordered.

 6. Lastly used a slicer for the Dates,which is in sync with all the Bar Graph and Pie Charts and all other visualizations.
   



