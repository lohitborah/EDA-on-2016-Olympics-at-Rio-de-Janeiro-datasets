# EDA on 2016 Olympics at Rio de Janeiro datasets:

## Summary

### Datasets description and link:

The two datasets used for analysis are from the 2016 Olympics at Rio de Janeiro. The first dataset "athletes" used is of 11,538 athletes, this dataset includes the name, nationality (IOC country code), gender, date of birth, height in meters, weight in kilograms, sport, and quantity of gold, silver, and/or bronze medals won. The second dataset "countries" contains information about the country name, IOC country code, population, and GDP per capita of the participating nations.

Dataset Link: https://www.kaggle.com/rio2016/olympic-games


### Process followed to import and combine the datasets:

The files were read as CSV into pandas data frames and then combined into one using merge function on the common column "IOC country code" using a left join. Pandas' pivot table function was also used to aggregate the final dataset at country and gender level for necessary analysis/visualization. 


### Analysis performed and interpretation of the results:

The analysis performed on the merged dataset and the interpretation of the results are as below:

1. Top five athletes details by no. of gold medals and medals tally plot: The top 5 players based on gold medals was found and their medal tally is plotted below. It was observed that "Michael Phelps" won the highest number of gold medals for the aquatics sports category. Two of the top five athletes are from USA and aquatic sports category.
2. Top five male and female athletes details and medals tally plots: The top 5 male and female players based on gold medals were found and their medal tally is plotted below. Two of the top five male athletes and three of the top five female athletes are from USA. "Katie Ledecky" is the top female athlete in the aquatics sports category.
3. Number of athletes participating from each country (Top 20 countries): USA, Brazil, and Germany have the highest number of participants in the 2016 Olympics.
4. Numbers of athletes participating in each sport: The highest number of athletes were in athletics followed by aquatics. 
5. Percentage of male and female athletes participating: ~45% of the total participating athletes in the 2016 Olympics were female.
6. Correlation coefficient and scatter plot of height vs. weight of all participating athletes by gender: The correlation coefficient of height vs. weight of all participating athletes is 0.76. 
7. Aggregating the data frame at the country level to do necessary analysis at the country level: The data frame was pivoted at the country level using the pivot table function of pandas.
8.Top 5 countries by total medals and medals tally plot: USA won the highest number of the total medal followed by Germany and UK.
9. Correlation coefficient and scatter plot of GDP per capita/Population vs. total medals won by a country: The correlation coefficient of 1st is 0.38 and for the 2nd is 0.32
10. Plot for medals tally of male and female athletes: The medals tally of male and female athletes by gold, silver, and bronze are plotted below.
