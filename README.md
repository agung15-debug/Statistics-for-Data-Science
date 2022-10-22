# Statistics for Data Science

## Descriptive Statistic ##
- Distribution

Distribution describes how values are distributed for a field. In other words, the statistical distribution shows which values are common and uncommon

- Skewness

Measure of the asymmetry of a distribution. A distribution is asymmetrical when its left and right side are not mirror images. A distribution can have right (or positive), left (or negative), or zero skewness. A right-skewed distribution is longer on the right side of its peak, and a left-skewed distribution is longer on the left side of its peak

- Correlation Coefficient

Correlation is a statistical measure that expresses the extent to which two variables are linearly related (meaning they change together at a constant rate). It’s a common tool for describing simple relationships without making a statement about cause and effect

## Inferential Statistics ##
Inferential statistics help you come to conclusions and make predictions based on your data.

When you have collected data from a sample, you can use inferential statistics to understand the larger population from which the sample is taken.

Inferential statistics have two main uses:
* making estimates about populations (for example, the mean SAT score of all 11th graders in the US).
* testing hypotheses to draw conclusions about populations (for example, the relationship between SAT scores and family income).


### Confidence Interval ###
In frequentist statistics, a confidence interval (CI) is a range of estimates for an unknown parameter. A confidence interval is computed at a designated confidence level; the 95% confidence level is most common, but other levels, such as 90% or 99%, are sometimes used

Step for calculate confidence interval on python :


### Hypothesis Testing ###
Hypothesis testing is an act in statistics whereby an analyst tests an assumption regarding a population parameter. The methodology employed by the analyst depends on the nature of the data used and the reason for the analysis.

Hypothesis testing is used to assess the plausibility of a hypothesis by using sample data. Such data may come from a larger population, or from a data-generating process. The word "population" will be used for both of these cases in the following descriptions.

## Outliers ##

- Difference Outliers & Anomalies

Outliers are observations that are distant from the mean or location of a distribution. However, they don’t necessarily represent abnormal behavior or behavior generated by a different process. On the other hand, anomalies are data patterns that are generated by different processes or wrong input.

- Example Outliers & Anomalies

Outliers:
When data has an average age of 28 years. However, the data has value grandfather is 70 years old and the baby is 1 year old. Data with numbers 70 and 1 are Outliers values. Because it is beyond average.

Anomalies:
If a data input enters a person's age of -20 or 10,000 years, it can be called an anomaly. Because it doesn't make sense that age is minus 10,000 years.

- How to check Outliers & Anomalies

Anomalies:
We can use the `describe()` function in Python. Then, we look at the maximum and minimum values. If there is something absurd in that value, it is called anomalies.

Outliers:
There are two ways to check outlier values:

a. Boxplot Diagram
Insert a boxplot diagram using the seaborn library. We can use syntax `sns.boxplot();`

b. Use IQR
Steps check outliers use IQR:
1. Choose the data to be checked for outliers
2. Finding first quartile and third quartile
3. Finding the IQR which is the difference between third and first quartile
4. Find lower and upper bound
5. Values below lower bound and above upper bound are outliers.

- Handling Outliers 

To handle outliers, we can select data above the lower bound and below the upper bound. In this way, outlier data will delete.


## Handling Missing Values ##

Before handling missing values, we need to determine the type of data to handle. Including numerical or categorical.
After this, we can choose way to handling missing values:

a. If numerical :
We can use median values ( Curtois or Skewness Distribution )

b. If categorical:
We can use mean values ( Normal Distribution )
