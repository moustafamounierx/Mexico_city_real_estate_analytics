# Mexico_city_real_estate_analytics
Objective: The primary objective of this section is to investigate and answer two key research questions regarding the Mexico real estate market
1-"Which state has the most expensive real estate market?" This involves analyzing how housing prices vary by state and identifying the most expensive regions for home purchases.
2-"Is there a relationship between home size and price?" This question aims to determine if the size of a house influences its price

**Research Question 1: Which state has the most expensive real estate market?**
-To address this, the mean house price for each state is calculated using the groupby method.
-A bar chart is then created to visualize these mean prices, sorted from highest to lowest.
-A new feature, "price_per_m2" (price per square meter), is calculated by dividing the house price by its area. This metric is considered more accurate for comparing houses of different sizes.
-The mean "price_per_m2" is then calculated for each state and visualized with another bar chart, again sorted from highest to lowest mean.
-Finding: The analysis reveals that Mexico City (Distrito Federal) is by far the most expensive market, especially when considering price per square meter, and many of the top 10 states by GDP are also among the most expensive real estate markets.

**Research Question 2: Is there a relationship between home size and price?**
-A scatter plot is used to visualize the relationship between "area_m2" (on the x-axis) and "price_usd" (on the y-axis).
-Initial Observation: The scatter plot shows a positive correlation, suggesting that generally, bigger houses tend to have higher prices, though there is considerable variation.
-To quantify this relationship, the Pearson correlation coefficient between "area_m2" and "price_usd" is calculated using the corr method. A coefficient over 0.5 indicates a moderate relationship.
-The analysis then narrows down to specific states to see if this relationship holds true everywhere:
        1-For the state of Morelos, a strong relationship between house size and price is observed, with a high correlation coefficient.
        2-For Mexico City (Distrito Federal), however, the scatter plot and correlation coefficient reveal a weak relationship between size and price.
