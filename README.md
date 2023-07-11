# Analyzing-and-Predicting-AQI-Data-through-Modeling
The project investigated the relationship between the Air Quality Index (AQI) and wealth in different counties in California. The research aimed to determine if lower-income communities are more prone to poor air quality due to a higher concentration of pollutant-emitting factories and power plants in their areas.

A multinomial logistic model was initially built to predict AQI categories, taking into account variables like county income, county income rank within California, and mean ozone concentration in 2020. However, despite achieving around 80% accuracy, the model was below the expected accuracy of a random baseline guesser with 6 classes (83%).

Two critical insights were gained from the data visualization: the similar distributions of normalized income and income rank, and a correlation between unemployment and income. This led to the decision to remove one of the variables (income rank) and include the number of unemployed people as an additional feature.

To improve the model, a switch was made from logistic regression to a Random Forest Classifier. Also, the income rank variable was dropped, and the number of unemployed individuals was incorporated. These modifications resulted in improved accuracy (from around 80% to 85%) and reduced error rates.

The results confirmed the hypothesis: counties in California with lower personal income tend to experience worse AQIs. This suggests that low-income communities are more vulnerable to the health implications of poor air quality. Further exploration is recommended to better understand the dynamics of this relationship and to uncover whether there is an unfair distribution of bad AQI within low-income areas. This can help guide efforts to alleviate the issue.
