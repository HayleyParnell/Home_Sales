# Home_Sales

Come along as I use my knowledge of SparkSQL to determine key metrics about home sales data. I use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

Usign SQLSpark I answer the following questions: 

1.The Average price for a four-bedroom house sold for each year is:

|sale_year|avg_price|
+---------+---------+
|     2019| 300263.7|
|     2020|298353.78|
|     2021|301819.44|
|     2022|296363.88|
+---------+---------+

2.What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? 

+----------+---------+
|year_built|avg_price|
+----------+---------+
|      2010|292859.62|
|      2011|291117.47|
|      2012|293683.19|
|      2013|295962.27|
|      2014|290852.27|
|      2015| 288770.3|
|      2016|290555.07|
|      2017|292676.79|
+----------+---------+


3. What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? 
+----------+---------+
|year_built|avg_price|
+----------+---------+
|      2010|285010.22|
|      2011|276553.81|
|      2012|307539.97|
|      2013|303676.79|
|      2014|298264.72|
|      2015|297609.97|
|      2016| 293965.1|
|      2017|280317.58|
+----------+---------+



4. What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? 
+----+----------+
|view| avg_price|
+----+----------+
|  99|1061201.42|
|  98|1053739.33|
|  97|1129040.15|
|  96|1017815.92|
|  95| 1054325.6|
|  94| 1033536.2|
|  93|1026006.06|
|  92| 970402.55|
|  91|1137372.73|
|  90|1062654.16|
|  89|1107839.15|
|  88|1031719.35|
|  87| 1072285.2|
|  86|1070444.25|
|  85|1056336.74|
|  84|1117233.13|
|  83|1033965.93|
|  82| 1063498.0|
|  81|1053472.79|
|  80| 991767.38|
+----+----------+
only showing top 20 rows

--- 1.4673829078674316 seconds ---


