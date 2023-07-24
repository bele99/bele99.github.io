---
title: "Statistics learning Part 1"
date: 2023-03-12 +0800
categories: [Statistic]
tags: [Statistic, Standard Deviation, Variance, Coefficient of Variation, Median Absolute Deviation]
---

## Standard Deviation

| Standard Deviation    |     Explain     |
|:----------------------------------|:-------------------------------|
| What?          |The standard deviation measures the average distance between each data point and the mean of the dataset.SD is the most common measure of variability.   |
|Formula|![Alt text](/images\2023\20230312\SD-Population.png) ![Alt text](/images\2023\20230312\SD-Smaple.png)|
| Interpretation          |Larger standard deviation: the numbers are more dispersed.Smaller standard deviation: the numbers group closely around the mean.|
| Advantage               | standard deviation over variance because it is directly interpretable.    |
| Disadvantage | Sensitive to outliers    |
| Application |1. commonly used in inferential statistics. 2. used in statistical analysis, quality control, and risk assessment. 3. used to determine the volatility of markets, financial instruments, and investment returns. |

## Variance
| Variance    |     Explain     |
|:----------------------------------|:-------------------------------|
|What?|A measurement used to identify how far each number in the data set is from the mean.|
|Formula|![Alt text](/images\2023\20230312\Variance-Population.png) ![Alt text](/images\2023\20230312\Variance-Sample.png)|
|Interpretation|=0: all of the values within a data set are identical. >0: all variances are the form of positive numbers. * Large variances: the numbers are far from the mean and each other. * Small variances: the numbers are closer toghter in value.|
|Advantage|It measures the spread of data points from the mean.|
|Disadvantage|Sensitive to outliers, like SD.|
|Application|1.Machine Learning: Used in Hypothesis Testing and Confidence Interval 2. Finance: Used to understand how risky and volatile the investment is, stability of mutual funds. 3.Forecasting: To make the weather forecast, projections about the company’s revenue. 4.Sports: Used to select the players in the team|

## Coefficient of Variation (CV)
| Coefficient of Variation (CV)    |     Explain     |
|:----------------------------------|:-------------------------------|
|What?|The CV is the ratio of the standard deviation to the mean, expressed as a percentage.|
|Formula|![Alt text](/images\2023\20230312\CV-Population.png) ![Alt text](/images\2023\20230312\CV-Smaple.png)|
|Interpretation|It measures the relative variability compared to the mean.|
|Advantage|Allows for comparison of variability between datasets with different means. The coefficient of variation has its edge over standard deviation when it comes to comparing data.|
|Disadvantage|Can be misleading when the mean is close to zero.|
|Application|Useful in comparing variability in datasets with different scales
commonly used in finance and biology.|

## Median Absolute Deviation(MAD)
| Median Absolute Deviation(MAD)    |     Explain     |
|:----------------------------------|:-------------------------------|
|What?|The MAD is the median of the absolute deviations from the median of the dataset. It quantifies the spread of data points around the median.|
|Formula|![Alt text](/images\2023\20230312\MAD.png)|
|Interpretation||
|Advantage|* Robust to outliers and extreme values. * Useful when the data is not normally distributed.|
|Disadvantage|May be less sensitive to subtle changes in data.|
|Application|Used in robust statistics, outlier detection, and data with non-normal distributions. MAD is a robust alternative to standard deviation, suitable for datasets |


## Reference
- https://www.shiksha.com/online-courses/articles/variance-and-standard-deviation/
- https://www.mathsisfun.com/data/standard-deviation.html
- https://365datascience.com/tutorials/statistics-tutorials/coefficient-variation-variance-standard-deviation/
- https://www.r-bloggers.com/2013/08/absolute-deviation-around-the-median/