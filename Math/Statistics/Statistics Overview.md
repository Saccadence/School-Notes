
Statistics: Measurement of the characteristics of a sample.

- Parameter: Overall of a variable being observed

- Statistic: A specific portion of a variable being observed

 

Types of Data

- Quantitative Data: Numerical

  - Discrete: Value of data is finite (0, 1, 2…)

  - Continuous: Value of data can have infinite number of possible values (Values between 0 - 1)

- Categorical Data: Names and Labels

  - Numbers can show up as labels (numbers on jerseys)

 

Simple Random Sample: n (sample size) measurements from a population is a subset of the population selected in a manner such that

- Every sample of size n from the population has an equal chance of being selected

- Every member of the population has an equal chance of being included in the sample

>  

Example of Simple Random Sample - Use a random number table to pick a random sample of 30 cars from a population of 500 cars

- Begin anywhere in table, pick groups of 3 numbers in that row

  - If above 500, disregard and move on

  - If below 500, save number and repeat until you have 30 cars

- Use calculator function - randInt(a,b,c)

  - a = 1 (start of range), b = (end of range), c = (number of random values needed)

  - Use with STO-\> and L1 to save to L1 for easy use

 

Frequency Distribution - Organize large data sets

- Shows how a data set is partitioned among all of several categories (or classes) by listing all of the categories along with the number of data values in each of them

  - Lower Class Limit - smallest numbers that can belong to different classes

  - Upper Class Limit - largest numbers that can belong to different classes

  - Class Boundaries - numbers used to separate classes, but without the gaps created by class limits

  - Class Midpoints - Values in the middle of the classes and can be found adding the lower and upper class limit and dividing by 2

  - Class Width - Difference between two consecutive class minimums or maximums

>  

- Construction of a Frequency Distribution

  - Determine the number of classes (between 5 and 20)

  - Calculate the class width by dividing max value-min value by number of classes (round up to 'beautiful' number) - ex. 18.2 --\> 20

  - Starting Point - Choose minimum data value or convenient value below it

  - Using starting point, create other lower class limits

  - List in vertical column and then list upper class limits

  - Take individual data value and tally in each appropriate class

 

- Relative Frequency Distribution

  - Includes the same class limits as a frequency distribution, but frequency of a class is replaced with a relative frequency (a proportion) or a percentage frequency (a percent)

    - Relative Frequency = Class Frequency/Sum of All Frequencies

    - Percentage Frequency = Class Frequency/Sum of All Frequencies x 100%

 

Exploratory Data Analysis -

Histograms

- A graph to help visualize the distribution of the data

- Bars of equal width drawn adjacent (unless there are gaps in data)

- Horizontal scale represents the classes of quantitative data values and vertical scale represents the frequencies

- Tells the same information as a frequency table, just in a different medium

 

- Relative Frequency Histogram

  - Shows the data relative to the size of the sample taken

    - Usually follow a bell curve

 

- Skewed Data

  - Positive Skew - Lower data right

  - Negative Skew - Lower data left

 

Dot Plots

- A graph where is data value is plotted as a point/dot along a scale of values

  - The higher the dots, the more of the same value

 

Stem and Leaf Plot

- Represents quantitative data by separating each value into two parts

  - Stem: Leftmost digit

  - Leaf: Right most digit

- How to Make:

  - Divide digits of each data value into two parts, the stem will contain digit(s) to the left of the right-most digit. The leaf will be the right-most digit.

  - Align all the stems in a vertical column from smallest to largest, draw a vertical line to the right of all stems.

  - Place all the leaves with the same stem on the same row and arrange them in increasing order.

  - Use a label to indicate the what the data represents. We include the decimal position in the label rather than with the stems or leaves. (ex. 18 books are in the store, 1\|5 --\> 15)

 

Multiple Bar Graphs

- Use to compare multiple sets of data

 

Pareto Chart

- Bar graph for qualitative data put in descending order according to frequency

 

Pie Chart

- Qualitative data as slices of a circle

  - Size is proportional to frequency count

    - Angle is calculated through percentage x 360 degrees

 

Misleading Graphs

- Non-zero Graphs

  - Can misrepresent differences in data through smaller min and max axis

- Showing one-dimensional data through three-dimensional data

  - E.x. Income difference shown with cubes

 

Chapter 3: Describing, Exploring, and Comparing

Measures of Center

- Measures and interpret the center of a data set including mean and median

- *Never* use average when referring to a measure of center. It is not used in statistics either in the community or professional journals

 

- Resistant

  - A statistic is resistant in the presence of extreme values (outliers) and does not cause it to change much

 

- Mean or Arithmetic Mean

  - Add all of the data values and divide by the number of data values

  - Important Properties:

    - Sample means drawn from the same population tend to vary less than other measures of center

    - The mean of a data set uses every data value

    - A disadvantage is that just one extreme value (outlier) can change the value of the mean drastically. (Non-resistant)

  - Notation:

    - ∑ - Denotes the sum of a set of data values

    - x - The variable usually used to represent the individual data values

    - n - Represents the number of data values in a sample

    - N - Represents the number of data values in a population

    - x̄ - (Pronounced "x-bar") The mean of a set of sample values

    - μ - (Pronounced "mu") The mean of all values in a population

 

- Median

  - The middle value of a set of data when sorted in an order of increasing or decreasing magnitude

  - Important Properties:

    - Does not change by large amounts when outliers are included, it is considered resistant

    - Does not directly use every data value

  - Notation:

    - x̃ - (Pronounced "x-tilde")

    - M or Med

  - Calculation:

    - If the number of data values is *odd*, the median is the exact middle of the set of data values in a properly sorted list

    - If the number of data values is *even*, the median is found by computing the mean of the two middle values in a properly sorted list

 

- Mode

  - Value(s) that occur with the greatest frequency

  - Important Properties:

    - Can be found with qualitative data

    - A data set can have no mode, one mode, or multiple modes

  - Finding the Mode:

    - When two data values occur with the same greatest frequency, each one is a mode and the data set is considered *bimodal*.

    - When more than two data values occur with the same greatest frequency, each is a mode and the data set is said to be *multimodal*.

    - When there is no data value repeated, we say that the is *no mode*.

 

- Midrange

  - The value midway between the maximum and minimum values in the original data set

    - Found by adding the min and max and dividing by 2

  - Important Properties:

    - Uses only maximum and minimum and is very sensitive to outliers (non-resistant)

    - Rarely used but:

      - Easy to compute

      - Helps reinforce the idea that there are different ways to define the center of a set of data values

      - Gets confused with the median so it is useful to define

 

- Rules:

  - Carry one more decimal place than is present in the original set of data values

  - Leave the mode(s) as is without rounding

 

- Mean from Frequency Distribution

  - Since there a no exact values to get a mean from, you must use the class midpoint to get a close approximation of the mean of a set of data

  - Multiply each frequency (f) and class midpoint (x), then add the products

  - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image1_2023-10-06T022759.1565598-0700.png" style="width:2.97222in;height:1.0625in" />

  - Calculator: 1-VarStats L1, L2

 

- Weighted Mean

  - Used when different (x) data values are assigned different weights (w)

  - Calculating:

    - Multiply all data values by their respective weight and add then add them all together

    - Divide the sum of all weighted values by the sum of the all weights used in the set of data (4+3+3+3+1, not 4+3+1)

    - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image2_2023-10-06T022759.1565598-0700.png" style="width:1.3125in;height:0.8125in" />

 

 

Measures of Variation

 

- Three important measures of variation:

  - Range, Standard Deviation, and Variance

- Round-off Rule:

  - When rounding the value, carry one more decimal place than is present In the original set of data

 

- Range - The difference between the maximum data value and the minimum data value

  - Very sensitive to outliers

  - Does not truly reflect the variation among all of the data values

 

- Standard Deviation - A measure of how much data values deviate away from the mean

  - Notation:

    - s = *Sample* standard deviation

    - σ = *Population* standard deviation

  - Formulas:

> <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image3_2023-10-06T022759.1565598-0700.png" style="width:3.125in;height:1.5in" />

- Important Properties of Standard Deviation:

  - Measure of how much data values deviate away from the mean

  - Value of the standard (s) in never negative and only zero when all of the data values are the same

  - The larger s equals, the greater the deviation

  - Standard Deviation (s) can increase dramatically with one or more outliers

  - Units of standard deviation are the same as the units of the original data values

  - Sample standard deviation (s) is a biased estimator of the population standard deviation (σ), which means that values of s do not center around the value of σ

 

- Variance - Measure of a set of values is a measure of variation equal to the square of the standard deviation

  - Sample Variance - s<sup>2</sup> = square of the standard deviation s

  - Population Variance - σ<sup>2</sup> = square of the population standard deviation σ

  - Important Properties:

    - Units of variance are the squares of the units of the original data values

    - Value of variance can increase drastically with the inclusion of the outliers (Non-resistant)

    - The value of the variance is never negative, only zero when all data values are the same number

    - Unbiased estimator of the population variance

  - Biased and Unbiased Estimators:

    - The sample standard deviation (s) is a **biased** estimator of the population standard deviation (σ)

      - The values of s do not tend to center around the value of the σ

    - The sample variance (s<sup>2</sup>) is an **unbiased** estimator of the population variance (σ<sup>2</sup>)

      - Values of s<sup>2</sup> tend to center around the value of σ<sup>2</sup> instead of systematically tending to overestimate or underestimate σ<sup>2</sup>

<!-- -->

- Empirical Rule w/ Bell-Shaped Distribution

  - 68% of all values within 1 standard deviation

  - 95% of all values within 2 standard deviation

  - 99.7% of all values within 3 standard deviation

>  

- Chebyshev's Theorem

  - Proportion of any data set lying within K standard deviations of the mean is always at least 1-1/K<sup>2</sup>, where K is any positive number greater than 1

    - For K=2, and K=3

      - At least 3/4 (75%) of all values lie within 2 standard deviations of the mean

      - At least 8/9 (89%) of all values lie within 3 standard deviations of the mean

 

- Coefficient of Variation (CV) - For a set of non-negative sample or population data, expressed as a percent, describes the standard deviation relative to the mean

  - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image4_2023-10-06T022759.1565598-0700.png" style="width:2.34028in;height:0.61806in" />

  - Round to one decimal place (e.g. 25.3%)

  - Used to compare variance between data sets

    - Example Interpretation of CV:

      - Although the standard deviation of 2.6 chocolate chips cannot be compared to the standard deviation of 0.00751 lb, we can compare the coefficients of variation, *which have no units*. We can see that **the numbers of chocolate chips(with CV=10.8%) vary considerably more than weights of Coke(with CV=0.9%)**. This makes intuitive sense, because variation among the numbers of chocolate chips is not a big deal, but if some cans of Coke were underfilled or overfilled by large amounts, the result would be angry consumers.

 

 

Measures of Relative Standing and Boxplots

 

- Key Concepts

  - Numbers showing the location of data values relative to the other values within the same data set

  - Percentiles, quartiles, and boxplots

  - Sorted set of data (as if doing median)

 

- z Scores

  - Number of standard deviations that a given value x is above or below the mean

  - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image5_2023-10-06T022759.1565598-0700.png" style="width:2.61806in;height:0.79861in" />

    - Round to two decimal places

  - Important Properties of z Scores

    - Numbers with no nits of measurement

    - Significant if z score is 2 or higher/-2 or below (z score)

    - Data value lower than mean will have a negative z score

 

- Percentiles

  - Measures of location, denoted P<sub>1</sub>, P<sub>2</sub>,…,P<sub>99</sub>, which divide a set of data into 100 groups with about 1% of the values in each group

  - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image6_2023-10-06T022759.1565598-0700.png" style="width:3.91667in;height:0.40278in" />

  - Round to nearest whole number

  - Notation

    - n = total number of values in the data set

    - k = percentile being used

    - L = locator that gives the position of a value

    - P<sub>k</sub> = the value of *k*th percentile

 

- Quartiles

  - Measures of location, denoted Q1, Q2, Q3, which divide a set into four groups with about 25% of the values in each group

    - Q<sub>1</sub> = Same value as P<sub>25</sub>, separates the bottom 25% of the sorted values from the top 75%

    - Q<sub>2</sub> = Same as P<sub>50</sub> and same as the median, separates the bottom and top 50% of a sorted set of values

    - Q<sub>3</sub> = Same as P<sub>75</sub>, separates the bottom 75% from the top 25%

  - Statistics defined using quartiles and percentiles

    - Interquartile Range (IQR) = Q<sub>3</sub> - Q<sub>1</sub>

    - Semi-interquartile Range = (Q<sub>3</sub> - Q<sub>1</sub>)/2

    - Midquartile Range = (Q<sub>3</sub> + Q<sub>1</sub>)/2

    - 10 - 90 Quartile Range = P<sub>90</sub> - P<sub>10</sub>

 

- 5 - Number Summary - 1-Var Stats on calculator

  - Minimum

  - First Quartile (Q<sub>1</sub>)

  - Second Quartile (Q<sub>2</sub>) - Median

  - Third Quartile (Q<sub>3</sub>)

  - Maximum

 

- Boxplot/Box-and-Whisker Diagram

  - Graph of data set that consists of a line extending from the minimum value to the maximum value, and a box drawn at the first quartile, median, and the third quartile

  - Procedure:

    - Find the 5-number summary

    - Construct a line segment extending from min to max

    - Construct a box (rectangle) from first quartile to third quartile and draw a vertical line to spilt the box at the second quartile

 

- Skewness

  - Boxplot is often used to identify skewness

    - Data is not symmetric and extends more to one side that to the other

  - Identifying Outliers

    - Find quartiles

    - Find IQR

    - Evaluate 1.5\*IQR

    - Outlier if a data value is above Q<sub>3</sub> by an amount greater than 1.5\*IQR or below Q<sub>1</sub> by an amount greater than 1.5\*IQR

    - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image7_2023-10-06T022759.1565598-0700.png" style="width:1.875in;height:0.4375in" />

 

- Modified Boxplot

  - A normal boxplot constructed with modifications such as:

    - A special symbol (asterisk or point) to identify outliers as defined above

    - The solid horizontal line extends only as far as the minimum data value that is not an outlier and the maximum data value that is not an outlier

>  

Basic Concepts of Probability

 

- Key Concepts

  - Learn how to interpret probability values, expressed within 0 - 1

    - The smaller the less likely

  - Odds and how they relate to probability

    - Used in events like lotteries and gambling

 

- Basics of Probability

  - Event - Collection of results or outcomes of a procedure

  - Simple Event - Cannot be further broken down into simpler components

  - Sample Space - All possible simple event, all outcomes cannot be broken down further

 

- Notation

  - P = Probability

  - A, B, C = Denote specific events

  - P(A) = Denotes probability of event A occurring

 

- Three Common Approaches to Finding the Probability of an Event

  - Relative Frequency Approximation of Probability

    - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image8_2023-10-06T022759.1565598-0700.png" style="width:3.04861in;height:0.36806in" />

  - Classical Approach to Probability (**Requires Equally Likely Outcomes**)

    - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image9_2023-10-06T022759.1565598-0700.png" style="width:3.04167in;height:0.35417in" />

  - Subjective Probabilities

    - The probability of an event is *estimated* by using knowledge of the relevant circumstances

 

- Simulations

  - Sometime none of the preceding three approaches can be used

  - A process that behaves in the same ways as the procedure itself so that similar results are produced

 

- Law of Large Numbers

  - As a procedure is repeated again and again, the relative frequency probability of an event tends to approach the actual probability

  - Caution:

    - Applies to behavior over a large number of trials and not individual outcome

    - If we know nothing about the likelihood of different possible outcomes, do not assume they are equal

 

- Complement

  - The complement of event A, denoted by A' or A<sup>c</sup>, consists of all outcomes in which A does not occur

 

- Actual Odds Against

  - The ratio P(A')/P(A), usually expressed as a:b

 

- Actual Odds in Favor

  - The ratio P(A)/P(A') expressed as a:b

 

- Payoff Odds

  - Against A occurring are the ratio of net profit to bet amount

    - (net profit):(amount bet)

 

 

Chapter 4: Probability

 

Addition Rule and Multiplication Rule

 

- Compound Event

  - Combining two or more simple events

 

- Addition Rule

  - P(A or B) = P(event A occurs or Event B occurs, or they both occur)

    - P(A) + P(B) - P(A and B)

 

- Disjoint (or Mutually Exclusive)

  - Events A and B are mutually exclusive if they cannot occur at the same time

 

- Multiplication Rule

  - P(A and B) = P(event A occurs in a first trial and event B occurs in a second trial)

  - P(B\|A) = Probability of Event B occurring after it is assumed that event A has already occurred

  - P(A and B) = P(A) \* P(B\|A)

 

- Independence and the Multiplication Rule

  - Independent

    - If one event does not affect the other when it occurs, they are independent of each other

      - Otherwise they are dependent

 

- Sampling

  - With Replacement: Selections are independent

  - Without Replacement: Selections are dependent

  - When sampling w/o replacement and the sample size is no more than 5% of the size of the population, treat the selections as being independent

 

- Redundancy

  - Increase the reliability of many systems

 

- Conditional Probability

  - A probability obtained with the additional information that some other event has already occurred

 

- Bayes' Theorem

  - Used for revising a probability value based on additional information

  - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image10_2023-10-06T022759.1565598-0700.png" style="width:1.77083in;height:0.42361in" />

 

- Prior and Posterior Probability

  - Prior - Initial value obtained before any additional information is obtained

  - Posterior - Value has been revised by using additional information that is later obtained

 

- Multiplication Counting Rule

  - First event occurs n<sub>1</sub> ways, the second event occurs n<sub>2</sub> ways, the third event occurs n<sub>3</sub> ways

    - The total is n<sub>1</sub> \* n<sub>2</sub> \* n<sub>3</sub> \* …

 

- Factorial Rule

  - The number of different arrangements of n different items when all n of them are selected is n!

 

- Permutations and Combinations

  - Permutations - different sequences of the same items are counted separately

  - Combinations - different sequences are counted the as the same

 

- Permutations Rule

  - When n different item are available and r of them are selected without replacement, the number of different permutations is given by -

    - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image11_2023-10-06T022759.1565598-0700.png" style="width:1.20833in;height:0.41667in" />

  - When items are identical, the number of different permutations (order counts) when n items are available and all n of them are selected without replacement

    - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image12_2023-10-06T022759.1565598-0700.png" style="width:0.875in;height:0.36806in" />

 

- Combinations Rule

  - When different items are available, but only r of them are selected without replacement, the number of different combinations (order does not matter) is found as follows -

    - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image13_2023-10-06T022759.1565598-0700.png" style="width:1.35417in;height:0.46528in" />

 

 

 

Chapter 5 - Probability Distributions

 

- Basic Concepts

  - Random Variable

    - A variable that has a single numerical value, determined by chance, for each outcome of a procedure

  - Probability Distribution

    - Give the probability for each value of the random variable

      - Expressed in the format of a table, formula, or graph

  - Discrete Random Variable

    - A collection of values that is finite or countable

  - Continuous Random Variable

    - A collection of values that is infinite or uncountable

 

- Probability Distribution Requirements

  - There is a numerical (not categorical) random variable, and its number values are associated with corresponding probabilities

  - The sum of probabilities must be 1 (or can be .999 or 1.001 due to rounding errors)

  - P(x) must be between or equal to 0 and 1

 

- Parameters of a Probability Distribution

  - Description of population, not a sample, so mean, standard deviation, and variance are parameters and not statistics

  - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image14_2023-10-06T022759.1565598-0700.png" style="width:2.77083in;height:1.56944in" />

>  

- <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image15_2023-10-06T022759.1565598-0700.png" style="width:2.77778in;height:0.77083in" />

 

- Expected Value

  - For a discrete random variable, where x is denoted by E, where E is the mean value of the outcomes

 

- Binomial Probability Distribution

  - Requirements:

    - A procedure has a fixed number of trials

    - They must be independent

    - Each trial must have all outcomes classified into two categories (success and failure)

    - The probability of success remains the same in all trials

  - Notation:

    - S = Success, F = Failure

    - P(S) = p, p = probability of success

    - P(F) = 1 - p = q, q = probability of a failure

    - n = the fixed number of trials

    - x = a specific number of successes in n trials, can be any whole number between 0 and n, inclusive

    - P(x) = probability of getting exactly x successes among the n trials

  - Methods of Finding Binomial Probabilities

    - <img src="C:\Users\Austin\Desktop\OneNote2MarkDown\Austin&#39;s_Notebook\Quick_Notes/media/image16_2023-10-06T022759.1565598-0700.png" style="width:3.02778in;height:0.70139in" />

    - Method 2: 2nd VARS (DISTR)

      - Binompdf(n,p,x) = the probability of getting exactly x successes among n trials

      - Binomcdf(n,p,x) = provides the sum of all probabilities from 0 through the specific value entered for x

 

 

 

Chapter 6 - Normal Probability Distributions

 

- The Standard Normal Distribution

  - Key Concepts

    - Bell-shaped

    - Mean = 0

    - Standard Deviation = 1

  - If a continuous random variable has a distribution with a graph that is symmetric and bell-shaped, it is a normal distribution

- Density Curve

  - The graph of any continuous probability distribution

  - Must have a total area of 1 under the curve

    - Correspondence between area and probability

- Uniform Distribution

  - Values of continuous random variable is spread evenly over the range of probabilities, rectangular

  - Equally Likely Events

- Finding Probabilities when given Z-Scores

  - If given x-values/z-values, use normalcdf(low, high, mean, std)

  - If we are given area, we need to find x-value/z-value, invNorm(cumulative area from left, mean, std)

- Critical Value

  - Z score on the borderline separating z scores that are significantly low or high

- Sampling Distribution of a Statistic

  - Distribution of all values of the statistic when all possible samples of the same size n are taken from the same population

- Sampling Distribution of the Sample Proportion

  - Distribution of the sample proportions with all samples having the same sample size n taken from the same population

- Estimator

  - A statistic used to infer the value of a population parameter

- Unbiased Estimator

  - A statistic that targets the value of the corresponding population parameter in the sense that the sampling distribution of the statistic has a mean that is equal to the corresponding population parameter


















