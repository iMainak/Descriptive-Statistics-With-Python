# Descriptive Statistics
Descriptive statistics identify important elements in a dataset
* Very important initial step
* Summarize data as it is not look for explanations
* Don't try and fit models to data
* Detect outliers
* Plan how to prepare a data (when you perform hypothesis testing or fit machine learning models is data preparation and cleaning)
* It is an important precursor to feature engineering

## Types Of Statistics:
<p align="center" width="100%">
          <img src= image/types.PNG>
</p>

## Types Of Analysis:
<p align="center" width="100%">
          <img src= image/analysis.jpg>
</p>

# Univariate

<p align="center" width="100%">
    <img src=image/univariate.PNG> 
</p>

## Measures of Freq:
How often a particular data point occurs with in your data.
* Tabular representation of your data and the corresponding frequencies
* Or you can use **Histograms** to visualize this

## Meausres Of Central Tendency:
Seek to find **that point arround which your data is centered**.

### **Mean**  
* Single best value to represent data, 
* Consider each and every point in data.
* Apply with discrete as well as continuos data.

***In present of outliers MEAN is so sensitive then MEDIAN***
### **Median**
* values such that 50% of the data on either side of the Median.
* Sort data then use middle element
* More robust outliers than mean.

### **Mode**:
* Most frequent value in dataset.
* Not great for continuos data.
* Higest bar in histogram
* Typically used with categorical data.
### Formula:
<p align="center" width="100%">
          <img src= image/StatisticsFormula.jpg>
</p>

### Example:
<p align="center" width="100%">
          <img src= image/meanMedianModeExample.jpg>
</p>
 
## Meausre Of Dispertion:

### **Range**
* Range ignores the mean and is surged by outliers - that's where variance comes in.
#### ***Variance and Bassels Correction***
* Variance measuer how much each data point varies from the mean and these mean deviation cal variance.
* Variance is the second most important number ti summarize the set of data points.
* We can improve our estimate of the variance by tweaking the denominators this is called BASSELS CORRECTION.

<p align="center" width="100%">
          <img src= image/basselsCorrection.png>
</p>

### **Standard Deviation**:
Standard deviation is the square root of variance, its a measure of how far your data lie from the mean.

<p align="center" width="100%">
          <img src= image/standardDeviation.jpg>
</p>

* Small std. Deviation means there are few points are far from the mean.
* Large std. deviation means there are many data points are far from the mean. 

### Inter-Quartile-Range (IQR):
* The IQR range is one of many measurements used to measure how spread out the data points in a data set are.
* It is best used with other measurements such as the median and total range to build a complete picture of a data set’s tendency to cluster around its mean.
* The **higher the IQR, the more spread out the data points**; in contrast, 
* The **smaller the IQR, the more bunched up the data points are around the mean**. 

* ***Q1 is the "middle" value in the first half of the rank-ordered data set.***
* ***Q3 is the "middle" value in the second half of the rank-ordered data set.***
* ***Q2 is the median value in the set.*** 

<p align="center" width="100%">
          <img src= image/iqr.png>
</p>

## Gaussian Distribution
* A distribution is a mathematical formula which tells how likeliy a particular value is to occur in your data. 
* It's important because it's gives you an idea what your data looks like. And properties in the real world such as height and weight of individuals and other natural properties can be represented by a normal distribution also know as Gaussian Distribution.

<p align="center" width="100%">
          <img src=image/normalDistributionFormula.png>
</p>

* In Gaussian Distribution 68% of the data points lie within within 1 std. deviation of the mean.
* 95% of the data will lie within 2 std. deviation of the mean.
* 99% of the data will lie within 3 std. deviation of the mean

## Confidence Interval
* **Population** is the all data out there in the universe
* **Sample** is a subset of the population
* **Sampling Distribution** is probability distribution of a population statistic given a particular sample.

<p align="center" width="100%">
          <img src= image/samplingdistributionmean.png>
</p>

# Skewness:
* Mainly used to find outliers on your data.
* A measure of asymetric arround the mean.
* So you have mean of your data , how is data distributed arround it.
* Normally distributed data  skewness is 0. it represents extreme values are equally likely on both sides of the mean.

<p align="center" width="100%">
    <img src=image/skewness.png> 
</p>

# Kurtosis:
* Kurtosis identifies whether the tails of a given distribution contain extreme values.
* How often extreme values (on either side of the mean)  occurs.
* Normally distributed data kurtosis is 3.
* Excess Kurtosis = kurtosis -3.
* Kurtosis about 3 indicates, **extreme events are more likely to occure** than in a normal distribution.
* A distribution with a negative kurtosis value indicates that the distribution has **lighter tails** than the normal distribution.

<p align="center" width="100%">
    <img src=image/kurtosis.jpg> 
</p>

# Bivariate
## Covariance
* Measures relationship between two variables specifically whether **greater value of one variable correspond to greater values in the other.**
* You get a sense of whether the vaiables move in the same direction.

## Correlation
* Similar to covariance; measures whether greater values of one variable correspond to greater values in the other. **Scaled to always lie between +1 and -1.**

***Independent variables have zero covariance and correlation***

<p align="center" width="100%">
    <img src=image/covarianceAndCorrelation.png> 
</p>

# Z-scores
* If you want to compare values across two categories or maybe two entirely different features, a common way to express your data is to use z-scores.
* Z-scores for any set of values is basically when you express every data points in terms of standard deviations from the mean.

<p align="center" width="100%">
    <img src=image/zscoreformula.jpg> 
</p>


* Positive values  above the mean
* negative values are below the mean
* Z-score value of 0 indicates that the value is exactly equal to the mean of our data
and the magnitude of the z-score tells you how many standard deviation away from the mean value is.
* z-scroe mean is 0 and std deviation 1
* Expressing data in terms of z-scores does not change the fundamental nature of our data, it just makes our data easier to work with, easier for comparisons across features.  