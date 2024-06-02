# Capstone-Module-2

In this Capstone project, I will analyze online retail shipping data. The main goal is to address the high number of deliveries that didn't arrive on time, which is almost half of the total shipments.

Here are the findings from analyzing the online retail shipping data:

* The dataset has 12 columns and 10,999 rows.
* There are no columns with missing (NaN) values.
* The ID column has unique customer identification numbers with no duplicates.
* The columns 'Warehouse_block,' 'Mode_of_shipment,' 'Product of importance,' and 'Gender' are text, while the rest are numbers.
* Columns like 'Customer_rating' and 'Reached.on.Time_Y.N' can be defined by specific codes.
* The correlation between variables is low, with no significant values above 0.05, so the analysis will focus on descriptive statistics.
* No missing or duplicate data was found using the isna(), isnull(), and duplicated() methods.
* No outliers were found using the interquartile range (IQR) method.
* Out of the 10,999 orders, more than half (6,563) were labeled as '1,' meaning they were not delivered on time.
