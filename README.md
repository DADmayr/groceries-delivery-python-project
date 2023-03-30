# Instacart Grocery Basket Analysis
Project concluded in the framework of the *CareerFoundry Data Analytics Programme*

## The Project
While the project is fictional, the subject of the analysis isn't. *Instacart* is an existing online grocery store operating through an app that has made their data available online. The project seeks to uncover more information about *Instacart's* sales patterns and assumes that *Instacart* stakeholders are most interested in the variety of customers in their database along with their purchasing behaviors. They want to target different customers with applicable marketing campaigns to see whether they have an effect on the sale of their products. The key questions they're interested in are:
+ What are the busiest days of the week and hours of the day (i.e., the days and times with the most orders)?
+ Are there particular times of the day when people spend the most money?
+ How can products be grouped into simpler price ranges?
+ Are there certain types of products that are more popular than others? Which departments have the highest frequency of product orders?
+ Is it possible to group different types of customers based on their ordering behaviour? E.g.:
  + What’s the distribution among users in regards to their brand loyalty (i.e., how often do they return to Instacart)?
  + Are there differences in ordering habits based on a customer’s loyalty status?
  + Are there differences in ordering habits based on a customer’s region?
  + Is there a connection between age and family status in terms of ordering habits?
  + What different classifications does the demographic information suggest? Age? Income? Certain types of goods? Family status?
  + What differences can be found in ordering habits of different customer profiles? 

## The Data
*Instacart* has provided a number of open-source datasets containing information about orders, products and departments. Additionally, *CareerFoundry* has provided a dataset on fictional customers. The data dictionary for the open-source data provided by *Instacart* is available [here](https://gist.github.com/jeremystan/c3b39d947d9b88b3ccff3147dbcf6c6b). The "Instacart Online Grocery Shopping Dataset 
2017” was last accessed from (https://www.instacart.com/datasets/grocery-shopping-2017) on 19.01.2023.

The data was analysed using Python. This repository makes available the Python scripts and the visualisations written/created to analyse the data as well as an Excel project report. 

## The Results of the Analysis
The analysis concluded with the following recommendations: 
1. As the busiest days are Saturdays and Sundays and most orders are placed between approx. 9am and 5pm, ads should be increased during those times. Email tagetting of customers could also take place on Fridays based on their recent purchases. This might lead them to buy more once they place their orders on Saturdays and Sundays.
2. Higher-priced products are ordered after midnight until ca. 3-4am. During this time, ads for the high-range products in Instacart's product palette could be placed. Between ca. 10am and 10pm ads for mid- and low-range products are the better choice. 
3. To group products into three categories, products with a price of max. 5$ were considered low-range, products with a price above 5$ and up to max. 15$ mid-range, and products above 15$ high-range. This categorisation showed that 67% of the products ordered fall into the mid-range category, 31% into the low-range category, and only 2% into the high-range category. Given that Instacart makes 98% of revenue with mid-range products, it could consider dropping high-range products from its products palette and focus fully on low- and mid-range products.
4. Produce and, interestingly, dairy eggs are by far the most popular departments. Further departments with orders above 2 million are snacks, beverages and frozen. When considering adding new products to their palette, Instacart should consider adding more products to those departments. Conversely, it is not recommended to add products to the five departments with the lowest number of orders. They are bulk, pets, alcohol, international, and babies. 
5. Regarding differences in customer types' ordering behaviour, five observations/recommendations were made:
  + First of all, it is noteworthy that most customers return to *Instacart* regularly, having a maximum number or orders above 10 and up to max. 40. *Instacart* could use this insight to specifically target the group of new customers (max. 10 orders placed) to tie them to *Instacart* and further increase the share of regular customers.
  + Secondly, the peak of orders for regular and new customers is on Saturdays whereas loyal customers peak on Sundays. *Instacart* could therefore specifically target loyal customers with ads on Saturdays and Sundays to nudge them to buy more on their most popular day.
  + Thirdly, the popularity of departments for loyal, regular and new customers is following a similar pattern with one exception: for bulk and babies the ratio of new customers is slightly lower. Hence, these departments are not a good choice for ads supposed to target new customers.
  + Forth, when looking at ordering habits across customer profiles and the four main US regions, the pattern is extremely similar across regions. Targeted advertisement based on geographical data at the regional level is therefore not recommended. However, this could be further investigated if disaggregated data for cities vs. periphery was available. 
  + Fifth, orders of customers with different profiles have similar patterns of ordering habits throughout the week. The only exceptions are low- and average-income elderly customers. Their peak days are Sunday and Thursday whereas for all other profiles, the peak days are Saturday and Friday. Hence, those customers could be specifically targeted on Saturdays/Sundays and Wednesdays/Thursdays with ads.
