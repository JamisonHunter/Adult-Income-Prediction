# Adult Income Predictions

The purpose of this notebook is to predict the income level of individuals using a machine learning algorithm. This algorithm will demonstrate insights with regard to what factors lead to which income level. The algorithm predicts two different levels of income. The first level is greater than 50,000 dollars per year. The second level is less than or equal to 50,000 dollars per year. From here, I will refer to these categories as being high income and low income respectively. Based on the below graph, we can see that low income represents a significantly larger portion of the target than high income. Therefore, any predictive algorithm should reach similar results.

![Income](income.png)

The adult income data set used here has a total number of 48,790 entries in the income column. Of these, 37,109 are low income and 11,681 are high income. This means that 79.1% are low income earners and 23.9% are high income earners. The algorithm that I use ought to end up fairly close to this.

# Correlations

One of the findings was that hours per week worked correlated slighltly with the level of education of the individual. A heatmap of all of the numerical column correlations can be seen below. Another one of the slightly more significant correlations was capital gains, which will end up being fairly significant as we move forward. 

![Correlation](corr.png)

Below I have a figure showing how level of education relates to hours worked per week. 

![Correlation](hourseducation.png)

# Gradient Boosting Model
