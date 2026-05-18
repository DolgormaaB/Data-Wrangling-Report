# Univariate Analysis 

## Categorical Variables 
When we talk about nominal data like room_type or borough, we can't calculate mean or standard deviation since they don't give us any particularly meaningful observations.

Instead, we look at frequencies, percentages, and mode. 

# Interpretation:

From our analyzed data and resulting graphs:

# Room Types:

From the graphs we can tell that the most common type of room is Entire Place (at 51.7%) followed closely by Private Room (at 45.9%). It's also clear that shared rooms are extremely rare, seeing as they make up just 2.26% of the listings.

# Boroughs:

Most of the listings are in Manhattan or Brooklyn, those two combined account for over 85% of the dataset's listings. Staten Island and the Bronx are much lower in terms of representation in listings.

# Continuous Variables

When it comes to continuous numerical data we can use all our mathematical oeprations like Central Tendency i.e mean and median, Variabiliy i.e Standarad Deviation and IQR, and Shape i.e skweness and kurtosis.

# Interpretation:

# 1. Price
i.) Central Tendency : the mean is much higher than the median indicating the data is heavily skewed by expensive outliers.

ii.) Variabliliy: the standard deviation is large i.e roughly $203 showing massive dispersion.

iii.) Shape : There is extremely high positive skewness (14.6) and kurtosis (373.7). It has a very long right tail (prices up to $8,000) making the median a much better measure of typical price than the mean. The high kurtosis value tells us that a majority of hosts are setting their rental prices at around the same rate of 100 to 150 (due to how 'spiky' our data is in the middle).

# 2. Rating :
i.) : The mean and median are almost identical, i.e about 4.

ii.) : The standard deviation stands at 0.57 which implies that most of the listings deviate from the 4.01 average. The IQR of 1 indicates that the middle 50% of all the airbnbs in NY are separated by just one star (mostly between 4 and 5)

iii.) : the distribution is relatively flat with a slight negative skew (-0.04) which means the scores are fairly spread otu but cluster a bit more toward the higher ratings. The negative kurtosis (-1.19) means the typical 'bell curve' peak isn't present here and has lighter tails (no extreme outliers past 3 to 5 range)

# 3. Availability :
i.) : The mean is 112 days, however the median is only 44 days. The mode is 0, meaning a huge chunk of properties are barely even available.

ii.) : The IQR here is 226 days, meaning that the availability varies widly between hosts.

iii.) : the skewness is positive (0.77), implying a heavy clustering near zero days avaialable. With a smaller peak at 365 days (the hosts that rent year round.)

# Cross Sectional Analysis

Here we're gonna group our data by a category and calculate things like **skewness** and **kurtosis**, together.

Let's group the Airbnb **prices** by **borough** to see how the distributions look across different areas of New York.



