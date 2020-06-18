## Variable Definitions:
*	**happiness**: The score is based on multiple independent variables that ranks 156 countries 
  by how happy their citizens perceive themselves to be.
*	**democracy**: An index created using the data from the Economist Intelligence Unit to express the quality of democracies. 
  Number between 0 and 100. The data is based on 60 different aspects of societies that are relevant to democracy, 
  i.e. universal suffrage for all adults, voter participation, perception of human rights protection, and freedom to form organizations and parties. 
*	**gini**: A measure of income inequality. The index number ranges from zero to one. 
  A zero meaning that there is no income inequality within the nation. 
  A high gini coefficient means that most the contries income goes to a small percent of the population.
*	**child_mortality**: This measures the number of deaths of children under 5 years of age, per 1000 live births. 
*	**refugee**: The share of refugees as a percentage of the total population of the country of residence.
*	**sanitation**: The percentage of people using at least basic sanitation service.
*	**women_edu**: The mean years a woman spends in school between the ages of 25 and 34 years. 
*	**men_edu**: The mean years a man spends in school between the ages of 25 and 34 years. 
*	**elder_child**: Measures the total dependency ratio in a country
  The percentage of the population composed of children under 14 and adults over 65 years.
*	**pop_den**: The average number of people per square kilometer.
*	**labour**: The percentage of people over 15 years old active in the labor force of the total population.
*	**region**: We have included a dummy indicator for regions, including Western Europe, Central and Eastern Europe, 
  Commonwealth of Independent States, Southeast Asia, South Asia, East Asia, Latin America and Caribbean, North America and ANZ, 
  Middle East and North Africa, and Sub-Saharan Africa.

## Data Cleaning: 
1. Transformed region names to numeric values to get all numeric variables
2. Aggregated the dataset by country using the mean. This dataset is pooled, meaning not every country has data for each
   point in time. In order for each country to have equal weight, the dataset is averaged by country.
3. Removed countries that do not have data for independent variables
4. Removed countries that do not have a democracy score
5. Replaced the numeric region values with names and created dummy variables for each region.
6. Dropped variables due to multicollinearity
7. Dropped unnecessary variables
