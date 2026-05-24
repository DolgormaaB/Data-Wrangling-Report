# Bivariate Analysis Report: AirBnb Dataset

In this section, we review different ways of bivariate analysis to understand the relationships between different variables in our dataset. We evaluate these relationships under two main categories: Quantitative and Qualitative variables.

---

## 1. Quantitative vs. Quantitative Correlation
When comparing two numerical variables, we choose our correlation measure based on whether we expect a linear or a non-linear relationship.

### A. Linear Correlation: Pearson's r
**Hypothesis:** There is a direct linear relationship between the total 'number_of_reviews' and 'reviews_per_month'.

**Interpretation:** To test whether these two numerical variables increase together at a constant rate, we use Pearson's correlation coefficient (r). This metric assumes a linear relationship. The test reveals a strong positive linear correlation between the two variables. This means that listings which accumulate a high total number of reviews also consistently maintain a high monthly review rate. The linear trend suggests a proportional relationship over time.

### B. Non-linear Correlation: Spearman's Rank & Kendall's Tau
**Hypothesis:** Listings with a higher 'number_of_stays' will have a higher 'number_of_reviews', even if the growth rate is not perfectly straight (non-linear).

**Interpretation:** Because real-world Airbnb data (like pricing or review counts) is often heavily skewed and doesn't follow a perfect straight line, I calculated both Spearman's Rank and Kendall's Tau correlation matrices. These methods evaluate monotonic relationships (whether variables move in the same direction, regardless of the rate). 

The results show an **almost perfect positive monotonic correlation** between the number of stays and the number of reviews. This confirms a strong consistency between customer activity and review behavior. While the exact linear rate might fluctuate, the rank order is preserved: more stays strictly lead to more reviews.

---

## 2. Qualitative vs. Qualitative Correlation
When comparing categorical variables, we use different metrics depending on whether the categories are purely binary or nominal.

### A. Binary Variables: Phi Coefficient
**Hypothesis:** Highly priced listings (Luxury Price) have higher availability (High Availability) than budget listings.

**Interpretation:** To test the association between two true binary variables (e.g., 'Luxury_Price' vs. 'High_Availability'), I generated a crosstab matrix and calculated the Phi coefficient. 

The resulting Phi value was very low. According to standard interpretation, this indicates a very weak or no association. This means that a high price does not mean the listing will have higher availability. There is very little correlation between a listing being classified as a luxury item and its calendar availability throughout the year.

### B. Nominal Variables: Cramer's V
**Hypothesis:** Types of rooms booked differ by location (Borough).

**Interpretation:**
To test whether room type differs by borough, I performed a chi‑square test of independence. The test was statistically significant, indicating that the distribution of room types is not independent of location.

To assess the strength of this association, I calculated Cramér’s V, which was 0.143. According to standard interpretation guidelines, this represents a weak association.

This means that although room type patterns vary across boroughs—as seen in the bar chart where Manhattan and Brooklyn have more entire apartments while Queens and Bronx have proportionally more private rooms—the overall strength of this relationship is weak. Location influences room type availability, but only to a limited extent. We can't confidently guess which type of room is booked by the majority of people just by looking at the borough.
