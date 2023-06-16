# Adult Income Predictions

The purpose of this notebook is to predict the income level of individuals using a machine learning algorithm. This algorithm will demonstrate insights with regard to what factors lead to which income level. The algorithm predicts two different levels of income. The first level is greater than 50,000 dollars per year. The second level is less than or equal to 50,000 dollars per year. From here, I will refer to these categories as being high income and low income respectively. Based on the below graph, we can see that low income represents a significantly larger portion of the target than high income. Therefore, any predictive algorithm should reach similar results.

![Income](income.png)

The adult income data set used here has a total number of 48,790 entries in the income column. Of these, 37,109 are low income and 11,681 are high income. This means that 79.1% are low income earners and 23.9% are high income earners. The algorithm that I use ought to end up fairly close to this.

# Correlations

One of the findings was that hours per week worked correlated slighltly with the level of education of the individual. A heatmap of all of the numerical column correlations can be seen below. Another one of the slightly more significant correlations was capital gains, which will end up being fairly significant as we move forward. 

![Correlation](corr.png)

Below I have a figure showing how level of education relates to hours worked per week. We can see that an educational level of nine correlates with the average of working forty hours per week, which makes sense. Paired with this figure is a distribution of the level of education of the individuals sampled for this data set. Since most people are well within this educational level of nine, most people work forty hours per week. Based on the below figure, we can also see that high income earners generally work higher hours since income correlates with level of education.

![Correlation](hourseducation.png)
![Correlation](education.png)

It will be important to note for the rest of this report how significant the correlation between high income earners and capital gains is. Of course, this is not some kind of shocking realization but I will often be using capital gains as a kind of pseudo-proxy for high income, which I believe is a justifiable approach based on the below figure.

![Correlation](incomecapitalgains.png)

This leads to what I believe is quite a fascinating correlation with income. If we compare the above figure and the below figure, what do we see? The two look quite similar when both marital status and income are compared to capital gains. This correlation also exists even when capital gains is factored out in exchange for factors like education and age. Income and marital status have a strong correlation with married people often being high income earners.

![Correlation](maritalstatuscapitalgains.png)

Let's take a look at a few other correlations! 

# Gradient Boosting Model
