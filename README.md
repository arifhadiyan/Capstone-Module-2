# Capstone Module 2

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

## Data Analysis

**Warehouse Block**

Our analysis shows that warehouse F has the most late deliveries. This might make it seem like warehouse F is the least efficient. However, a closer look shows that it's not the worst.

For example, warehouse B has only 16.4% of on-time deliveries but 16.8% of late deliveries. Only warehouse A has a "surplus," meaning it has a higher percentage of on-time deliveries (17.1%) compared to late deliveries (16.4%).

To improve efficiency in warehouses without an on-time delivery surplus, the transport manager could increase loading space to speed up loading. The warehouse location also affects delivery times. If a warehouse is in a hard-to-reach area, it can delay deliveries. Getting feedback from drivers about warehouse locations could help improve delivery efficiency.

**Mode of Shipment**

After analyzing the Mode of Shipment, we can see that shipping is often late compared to other methods. Shipping is also the most commonly used method. To fix this, road transport could be a good option since it has the fewest late deliveries. But road transport can't be used if the shipment has to cross water.

Air transport is the next best option. It can be expensive, but it has fewer late deliveries than shipping. Shipping is cheaper and can cross seas, but it has more late deliveries.

**Customer Rating**

Products with a customer rating of 1, which shows the lowest satisfaction, surprisingly have the most on-time deliveries (value of '0'). On the other hand, products with a rating of 5, the highest satisfaction, have the fewest on-time deliveries. This suggests that a high rating reflects overall customer satisfaction, not just timely delivery.

Several factors can affect customer ratings even if the delivery is on time, such as:

* The delivery was on time, but the quantity was incorrect.
* The product was damaged during delivery.
* The product was different from what the customer ordered.
* The product was not of the expected quality.
* There was a lack of proper updates or tracking information during shipping.

**Prior Purchases**

The graph and the chi-square test show that orders with three prior purchases are most often late. Also, the rate of late deliveries goes down as the number of prior purchases goes up. The chi-square test confirms that there's a significant link between the number of prior purchases and on-time delivery.

## Conclusions

* Each warehouse has its own issues, like Warehouse F handling a large volume of products. These issues can affect on-time deliveries, so improving warehouse processes is important.
* Every shipping method has its own challenges, so a good plan is crucial to meet the promised ETA.
* Customer ratings might not show the whole process, but problems like mistakes during picking can lead to dissatisfaction and low ratings, even if the delivery was on time.
* Regular orders help drivers get familiar with the area, increasing the chances of on-time deliveries.

## Recommendations

* Keep a surplus percentage in each warehouse block to avoid shortfalls.
* Have Warehouse A share its loading methods and layout plans with other warehouses. Regular comparisons can lead to improvements across all warehouse locations.
* Add extra time to the Estimated Time of Arrival (ETA) to reduce the risk of late deliveries.
* Work with a Third Party Logistics (3PL) provider known for on-time deliveries.
* Use real-time tracking for the transport team to monitor shipments and quickly address any delays.
* Use advanced routing software to find the best routes, considering traffic, road conditions, and weather. This can help reduce transit times and increase on-time deliveries.
* Implement a tracking system for customers to monitor their deliveries. This transparency can improve customer satisfaction.
* When possible, use the same driver or 3PL for repeat customers. This helps the driver get familiar with the location and speeds up delivery.
