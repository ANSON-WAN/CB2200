# CB2200 PALSI 2024-2025B, Anson Section

Hi! Everyone. It is so great to see you guys at this palsi section. You guys make not just a first step to get a good grade in this course.

~~Even I particularly choose the friday course and begin at friday 7:00 pm. You guys are still coming~~

Let me introduce myself first. My name is Anson. I am currently stuudying in computaional finance and fincance technology , double major in information mangement (business intelligence)

I think we could make something fantastics and create some good job together in this semester :joy:

Last semester, This course exam have be heavily rely on your understanding of concepts and my palsi friends told me that it is the hardest one in recent year. It indicates the following things:
- You need to understand the concepts deeply
- Understand why the question is and how to answer correctly
- Make sure you do the exercise every week as it will be overloaded at the semester end (trust me)(Last semester, I saw that my palsi friends can not finished the revision)

As it is first class, I will mainly focus on concept. 
I will also introduce some things you gonna know for your fully understanding, like numeric elemetary method, set theoty, python programming, matlab calculation, and some data science concepts. It is totally optional. 

My goal is to make sure you have a fully solid background not only for this class and even get the advanced statistics concepts and data analysis methdology.

**It is not finished as Cityu only give me 1 paid hour for preparing. I will continuously to update when I was free**

The role of probability theory
---
prob analysis predice and help to make decision in real world
real world get data and then establish statistics
statistics model the prob analysis

Understanding of the Syllabuds
---

| Topic | Contents |
| ----------- | ----------- |
| Introduction to Statistics | • <mark style="background-color: #FFFF00">Types of variables/ Organizing and visualizing data/ Measures of central tendency/ Measures of variation</mark> / Exploring numerical data/ Use of Excel |
| Basic Probability | <mark style="background-color: #FFFF00">• Basic probability concepts /• Conditional probability /• Counting rules </mark>|
| Discrete and Continuous Probability Distributions | Text |
| Sampling Distribution | Text |
| Confidence Interval Estimation for the Population Mean | Text |
| Hypothesis Testing for the Population Mean | Text |
| Confidence Interval Estimation and Hypothesis Testing for the
Population Proportion | Text |
| Simple Linear Regression | Text |

---

### Intitiation : What is Statistics 
Statistics, Data Science, Machine Learning , Ai = Use data gather insight and make decisions
- Prob = Random Process to get data = Randomness
- Statistics understand the process and make predictions

| Phenonemon | Result |
| ----------- | ----------- |
| When you want to find the random result of one thing | it is prob |
| When you want to understand the result | this is stat |

#### Statistics Types:
1. Descriptive Statistics 
: focuses on summarizing and organizing data in a meaningful way
- Measure of Central Tendency : measures indicate the center or typical value of a dataset
    - mean
    - median
    - mode
- Measures of Dispersion : describe the spread or variability of the data
    - Range
    - Variance
    - Standard Deviation
- Distribution Shapes
    - Normal Distribution
    - Skewness (left or right skewed)
    - Kurtosis (tailedness)
- Data Visualization
    - Charts and Graphs
    - Summary Tables
2. Inderence Statistics : A type of statistics that uses sample data to draw conclusions about a larger population
## Ch.1 Basic Concept

### 1. Sample Space
- List/Set of possible outcomes (All the possible outcome)
It is like : [1,2,3,4,5,6] when you throwing a dice once

It have three property:
- Mutually exclusive (互相排斥) (you can not have two things at same time)
- Collectively exchaustive (全面詳盡) (It represent all possible)
- At the "right" granularity (Only look for suitable size of object)

Basic sample formatting
    1.Tree
    2.Table
    3.Continuous Distribution like format for continuous data

### 2. Event
- subset of sample space 
It is like : Getting 1 from [1,2,3,4,5,6] when you throwing a dice once

### 3. Axioms
What we use to induce many theorem in prob theory
    - P(A) >= 0
    - P(All) == 1
    - Addictivity : P(A and B) = P(A) + P(B) <=> (This math symbol mean if and only if) P(A) + P(B)

Just need to know, you will not induce them as you are BBA student

### 4. Common prob induced from Aioms
- **P(A or B or C) <=> A and B and C are disjoint == P(A) +P(B) + P(C)**
- p({A_1,A_2,A_3,A_4}) == P(A_1 + A_2 + A_3 + A_4)
- B include A >>> P(B) >= P(A)
- **== P(A OR B) = P(A) +P(B) - P(A AND B)**
- P(infinite of event with all using and) == 0

### 5. Counting
- Permutatuins : repetition is prohibited
- Combinations n!/(k!(n-k)!)
- Partitions : We try to break down a large things into smaller part, and then apply the things you want to find / all possibility of things
    - 52 cards, Each player gets an ace.
    - 4 * 3 * 2 * (48!/((12!)(12!)(12!)(12!)))/(52!/((13!)(13!)(13!)(13!)))
    - 4 * 3 * 2 is distributing the ace
    - 48!/ ((12!)(12!)(12!)(12!)) is other cards gived to others
    - Paritions is like divide a large part according to the number of people or anything you want to find, to break down of it into smaller part. It is not probability that range from 0 to 1.
- Number of subsets : It is liked ask you how many possibility of the questions
    - if you must throw dice twice, you will have 6*6 number of subset. If you do not throw any dice or one dice is possible, it will have 1 + 6 + 6*6 subset.
    - if he ask you how many number of subeset it creates of throwing 5 coin, it should be 2**5 
- Binomial prob : All is independence, it simplify things as true and false, and ask you the prob of it. 
    - (n C k) * p^k * (1-p)^(n-k) for it do not have specific order
    - p^k * (1-p)^(n-k) for it have specific order
---
**A very intutive way to do counting problem, use the things you want to find / all possibility of things**

### 6. Random variable
- We use X, Y, Z , these capital letter to represent random variable
- x, y, z is numer value as rule of thumb 
- It associates a value to every possible outcome
- P_X(x) = P(X = x) 
- Sum of all value of random variable should be one

| Example | Description |
| ----------- | ----------- |
| P(X = 4) in throwing a dice once | find the prob of throwing the value 4 |
| P(X = 4) in throwing two dice | Find the prob that two dice sum is 4 |

### 7. Five number summary
- The minimum
- The first quartile (Q1)
- The median, or second quartile (Q2)
- The third quartile (Q3)
- The maximum 
The five number summary is useful because it gives you an **overall idea of the distribution of your data**, from the extreme values to the center. You can visualize it with a box plot.

## Ch.2 Probability

Probability uses math to quantify uncertainty.
The probability that an event will occur is expressed as a number between 0 and 1.


| Prob value | Outcome |
|------      | ------|
| 0          |  impossible |
|  1         | certainly happen |
| 0 < 1      | May happen |

### 1. Random experiment
A process whose outcome cannot be predicted with certainty. Probability deals with what statisticians call random experiments

- The experiment can have more than one possible outcome.
- You can represent each possible outcome in advance.
- The outcome of the experiment depends on chance.

### 2. Multiple event with probability

**This is the first difficulty thing in CB2200**

#### Two Types of event


| Events Type | What it is | Example |
| -------- | -------- | --------|
| Mutually exclusive events |  they cannot occur at the same time | Throwing a dice, you only get one outcome. This is mutully exclusive |
| Independent events | the occurrence of one event does not change the probability of the other event | the occurrence of one event does not change the probability of the other event |

Why is it important
- It will affect how you deal with probability
- Multiplation law for independent event
- Addition rule for mutually exclusive events


| Rules | Usage | Formula |
|-----|------|-------|
| Multiplation law  | for independent event | P(A and B) = P(A) * P(B) |
| Addition rule  |  for mutually exclusive events | P(A) + P(B) |
| Complement rule | It is used to calculate the prob of its complement event| P(~A) = 1 - P(A) |

Example : Calculate the prob of a dice getting 1 and 4.
- P(A) + P(B) = P( A and B)
- A is the event of getting 1 and B is the event of getting 4
- It is beacuse they are mutullly exclusive, so we could add them up.
- Calculation : 1/6 + 1/6 = 2/6

Example : Throwing Two coins and they both get head
- P(A) * P(B) = P( A and B)
- 1/2 * 1/2 = 1/4
- It is because they are independent event, so we could multiple them

### 3. Dependent Probabillity
- Conditional probability refers to the probability of an event occurring given that another event has already occurred. 
- allows you to describe the relationship between dependent events, or how the occurrence of the first event affects the likelihood of the second event

### 4. Conditional Probability
- Prob of one event A happene given that another eveent B happen
- Important math formular : **P(A|B) == P(A and B)/ P(B)** and **P(B|A) == P(A and B)/ P(A)**
- P(B|A) = P(A and B) / P(A)  **==** P(A and B) = P(A) * P(B|A)
- They are same
- For your reference, P(A|B) = = P(A and B) / P(B), what happen first, put what event to divide. 

### 5. Total prob theorem (Optional)
- P(B) = Can be formmed by adding all P(A_i) * P(B|A_i)
- It is like we get many part of event A and many part of event A have some weighted on the happened of event B like 0.1 = P(A_1 and B) , 0.2 = P(A_2 and B), we try to use it to guess the prob of event B
- We use it to establish another event prob B
- P(B) = P(B∣A_1)*P(A 1)+P(B∣A_2)*P(A_2)+ ......
- I just skip the last part , but you can trt to induce it by M.I which finding the first one, then assume N case, finally check the N+1 case. It is the math way to prove something

### 6. Bayes' rule (Optional)
- Based on Total prob theorem and conditional prob
- We found what is the prob of event B by summarizing event P(A_i and B)
- Revised back and use conditional prob, P(A_i|B)
- It is the foundamental of Bayesian inference, we use inference as it is based on guess . It may not be True. It is not the same as statistcs
- We model B from A_i and then use B to inderence A_i
- It is a systematic approach for incorporating new evidence. 
- In Bayesian statistics, prior probability (先驗機率) refers to the probability of an event before new data is collected. Posterior (後發事件) probability is the updated probability of an event based on new data. 
- Bayes’s theorem lets you calculate posterior probability by updating the prior probability based on your data.

## Ch.3 Probability of distribution
We use probability distributions to model different kinds of datasets.

We identify significant patterns in their data.

Probability distribution describes the likelihood of the possible outcomes of a random event.

### 4 types of common discrete probability distribution
- Uniform 
- Binomial
- Bernoulli 
- Poisson

| Probability distribution | Usage | Example |
|-----|-----|------|
| Uniform | All event have same probability. | Throwing a fair dice |
| Binomial | True or False | Eat lunch or not eat lunch |
| Bernoulli | Sequence of True or False | Eat lunch or not eat lunch on multiple days |
| Poisson | during a specific peorod, how often it will happen | How many phone call during one hour |

Parameter: A characteristic of a population

Remark on Binomial and Bernoulli 
- The experiment consists of a number of repeated trials.
- Each trial has only two possible outcomes.
- The probability of success is the same for each trial.
- And, each trial is independent.

Remark on Possin distribution
- The number of events in the experiment can be counted.
- The mean number of events that occur during a specific time period is known.
- Each event is independent. 

### Continuous probability distributions
| Functions | Features |
| --------- | -------- |
| Probability Mass Functions (PMFs) | represent discrete random variables |
| Probability Density Functions (PDFs) | represent continuous random variables | 

Continuous probability distribution is used for continuous type of data. As it calculate the mass. Continuous type of data never can be measured by absolute number.

Like your height will always have some deciminal value at measuring. You cannot say you are absolutely 180cm.  

#### Very common and useful continuous probability distribution : Normal distribution
normal distribution is a continuous probability distribution that is symmetric about the mean and bell-shaped

Features
- The shape is a bell curve
- The mean is located at the center of the curve
- The curve is symmetrical on both sides of the mean
- The total area under the curve equals 1

Empirical Rule
- 68% of values fall within 1 standard deviation of the mean
- 95% of values fall within 2 standard deviations of the mean
- 99.7% of values fall within 3 standard deviations of the mean
- one sd mean one z-score in the calculation

 ## Ch.4 Sampling

| Data Type | Explain | 
|----|----|
| Population | every possible element that you are interested in measuring, or the entire dataset that you want to draw conclusions about |
| Sample | subset of a population |

Sampling is the process of selecting a subset of data from a population.

- It’s often impossible or impractical to collect data on the whole population due to size, complexity, or lack of accessibility 
- It’s easier, faster, and more efficient to collect data from a sample
- Using a sample saves money and resources 
- Storing, organizing, and analyzing smaller datasets is usually easier, faster, and more reliable than dealing with extremely large datasets 

---------

### 4.1. Representative sample (Optional)

It accurately reflects the characteristics of a population. 

This is what simple that you are looking for.

###  4.2. Sampling Process / Step (Optional)
1. Identify the target population
2. Select the sampling frame : list of all the individuals or items in your target population. More specific than population. It will include elements apart from this set
3. Choose the sampling method
    - non-probability sampling 
        - Convenience sampling : conducting a convenience sample involves collecting a sample from somewhere convenient to you
        - Voluntary response sampling : A voluntary response sample consists of members of a population who volunteer to participate in a study.
        - Snowball sampling : researchers recruit initial participants to be in a study and then ask them to recruit other people to participate in the study. 
        - Purposive sampling : select participants based on the purpose of their study
    - probability sampling
        - Simple random sampling : selected randomly and has an **equal chance** of being chosen
        - Stratified random sampling : you divide a population into groups, and randomly select some members **from each group** to be in the sample
        - Cluster random sampling : you divide a population into clusters, randomly select certain clusters, and include all members from the chosen clusters in the sample
        - Systematic random sampling : you put every member of a population into an **ordered sequence**. Then, you choose a random starting point in the sequence and select members for your sample at regular intervals
4. Determine the sample size 
    - Sample size helps determine the precision of the predictions you make about the population. 
    - In general, the larger the sample size, the more precise your predictions. However, using larger samples typically requires more resources. 
5. Collect the sample data

### 4.3. Infer population parameters with the central limit theorem
central limit theorem states that the sampling distribution of the mean approaches a normal distribution as the sample size increases.

as your sample size increases, your sampling distribution assumes the shape of a bell curve.

as you sample more observations from a population, the sample mean gets closer to the population mean.

### 4.4. Conditions about using Sampling
- Independence : must be independent of each other
- Randomization : sample data must be the result of random selection
- Sample size : sufficiently large
- A sampling distribution is a probability distribution of a sample statistic.

### 4.5. Sampling distribution
**Sampling distribution represents the possible outcomes for a sample statistic**

- You can use a sampling distribution to represent statistics such as the mean, median, standard deviation, range, and more
- We compute sample statistics like the mean to <mark style="background-color: #FFFF00"> estimate the corresponding population parameter </mark>
- Sampling distributions describe the uncertainty associated with a sample statistic, and help you make proper statistical inferences.
- Standard error is the sd of sd
- Sampling distribution is the probability of all the sample mean / the standard deviation of a sample statistic

## 5. Confidence intervals
- An interval estimate uses a range of values to estimate a population parameter.
- help describe the uncertainty surrounding an estimate. 
- Technically, 95% confidence means that if you take repeated random samples from a population, and construct a confidence interval for each sample using the same method, you can expect that 95% of these intervals will capture the population mean. You can also expect that 5% of the total will not capture the population mean. 
- Confidence Level : The confidence level represents the probability that a confidence interval will contain the true parameter value. Common confidence levels are **90%, 95%, and 99%**.
- The confidence level refers to the long-term success rate of the method, or the estimation process based on random sampling. 
- Imagine you take 20 random samples of 100 penguins each from the penguin population, and calculate a 95% confidence interval for each sample. You can expect that approximately 19 of the 20 intervals, or 95% of the total, will contain the actual population mean weight of 31 pounds. One such interval will be the range of values between 28 pounds and 32 pounds. 
- Statistical Significance
    - Definition: Statistical significance indicates whether the observed effect or relationship in the data is unlikely to have occurred by random chance alone, based on a predetermined significance level (e.g., α = 0.05).
    - Usage: Helps in deciding whether to reject the null hypothesis. If the P-value is less than α, the result is considered statistically significant.

-------
Step of calculation
1. Identify the statistic type (population/sample?)
2. if it is sample use z/t ?
3. what is the confidence level ?
4. Find the margin of error 

--------
### Common Misconception

- Misinterpretation 1: 95% refers to the probability that the population mean falls within the constructed interval (In strictly, the population will not change, this statement seems like it would be changed.)
- Misinterpretation 2: 95% refers to the percentage of data values that fall within the interval 
- Misinterpretation 3: 95% refers to the percentage of sample means that fall within the interval 
- Remark : There is no assumed relationship between confidence interval and confidence level. 

----------

We can say that we have 95% confident that the real population mean is in the interval

reflects how confident you are that the interval contains the true parameter, not the probability that the parameter lies within that specific interval after it has been calculated.
Once the interval is calculated, it either contains the true mean or it does not; the confidence level refers to the long-run performance of the method used to create the interval.

----------
### Construct a confidence interval for a small sample size (n<30)
| Sample size |  Method |
| ----- | ----- |
|   N> 30 | Z-DISTRIBUTION |
|   N <30 | T-DISTRIBUTION (typically, not a must) |

When constructing a confidence interval, first, identify a sample statistic; second, choose a confidence level; third, find the margin of error; and fourth, calculate the interval.

##### Remark
- If Sample size enough, we can use z-distribution what ever the prob distribution it is
- The t-distribution is specifically used when the population standard deviation is unknown. (Unknown Population Standard Deviation)
- The sample should be randomly selected from the population to ensure that it is representative.
- The observations in the sample should be independent of each other.

| Feature	| t-Distribution	| z-Distribution |
| --------   |  ---------- |  ----------- |
|Sample Size	|Typically used for small samples (n < 30). |	Used for large samples (n ≥ 30) or when the population is known to be normal. |
| Population Standard Deviation |	Used when the population standard deviation is unknown. |	Used when the population standard deviation is known. |
|Shape	|Flatter and wider than the z-distribution, with heavier tails. |	More peaked and narrower than the t-distribution. |
|Degrees of Freedom	|Depends on the sample size (df = n - 1). |	Does not depend on sample size; it is a standard normal distribution.|
|Use in Hypothesis Testing	|Used for testing hypotheses about means when the sample size is small or standard deviation is unknown. |	Used for testing |hypotheses about means when the sample size is large or standard deviation is known.|
|Critical Values|	Critical values vary based on degrees of freedom.	| Fixed critical values based on the standard normal distribution (z-table). |
|Robustness	|More robust to violations of normality for small samples, especially with larger sample sizes.|	Less robust; assumes normality in the population.|

**In practice, the choice between the two distributions often hinges on sample size and whether the population standard deviation is known.**

**Reason to use t-distribution : Smaller sample mean more uncertainty involved in estimating the standard error for small sample sizes**

### Margin of error
The margin of error (MoE) is a statistic that quantifies the amount of random sampling error in a survey's results. It provides a range around a sample estimate (like a mean or proportion) within which the true population parameter is expected to fall, given a certain level of confidence.
- The margin of error indicates how much the sample results may differ from the true population value.
- Usage : A margin of error of ±3% means that if the survey result is 50%, the true population percentage is likely between 47% and 53%.
- helps to understand the reliability and precision of survey results

## 6.Hypothsis Testing
- hypothesis testing uses sample data to evaluate an assumption about a population parameter. 
- conduct a hypothesis test to decide whether the evidence from their sample data supports either the null hypothesis or the alternative hypothesis
- Revise : Statistics significance : the claim that the results of a test or experiment are not explainable by chance alone.

Steps of doing hyphosis testing
1. State the null hypothesis and the alternative hypothesis.
2. Choose a significance level.
3. Find the p-value.
4. Reject or fail to reject the null hypothesis.

| Types| Effects|
|----|----|
| Null hypothesis | “no effect,” “no difference,” “no relationship,” or “no change.” |
| Alternative hypothesis | “an effect,” “a difference,” “a relationship,” or “a change.” |

### 6.1 Hypothesis testing error
hypothesis testing is based on probability, there’s always a chance of drawing the wrong conclusion about the null hypothesis.

When you decide to reject or fail to reject the null hypothesis, there are four possible outcomes :

- Reject the null hypothesis when it’s actually true (Type I error)
- Reject the null hypothesis when it’s actually false (Correct)
- Fail to reject the null hypothesis when it’s actually true (Correct) 
- Fail to reject the null hypothesis when it’s actually false (Type II error)

Two important concepts in hypothesis testing error
1. Alpha : Your significance level, or alpha (α), represents the probability of making a Type I error
2. Beta : probability of making a Type II error is called beta (β), and beta is related to the power of a hypothesis test (power = 1- β)

Solutions :
Type I error : To reduce the risk of a Type I error, one can choose a lower significance level (α), which makes it harder to reject the null hypothesis.
Tyoe II error : To reduce the risk of a Type II error, researchers may increase the sample size or the significance level, but this can increase the risk of Type I errors.

Therefore, you can choose to reduce one error risk at one time. Considering the risk and benegit of each error will incur, then you will make a right choice. 

### 6.2 Hypothesis testing Best practice
Two main rules for drawing a conclusion about a hypothesis test: 
- If your p-value is less than your significance level, you reject the null hypothesis.
- If your p-value is greater than your significance level, you fail to reject the null hypothesis. 

The P-value quantifies the strength of the evidence against the null hypothesis. It represents the probability of observing results as extreme as the ones obtained, assuming the null hypothesis is true.

1. If your P-value is less than your significance level (P < α):
Interpretation: This indicates that the observed data is very unlikely under the assumption that the null hypothesis is true. Since the probability of observing such extreme results is low, we have sufficient evidence to reject the null hypothesis.
Conclusion: Rejecting the null hypothesis suggests that there is a statistically significant effect or relationship present in the data.
2. If your P-value is greater than your significance level (P > α):
Interpretation: This indicates that the observed data is consistent with the null hypothesis. The probability of observing such results is relatively high under the null hypothesis, suggesting that we do not have enough evidence to reject it.
Conclusion: Failing to reject the null hypothesis means that the evidence is insufficient to support the alternative hypothesis. This does not prove that the null hypothesis is true; it simply indicates a lack of evidence against it.

| p-value and significance level | Interpretation | Conclusion |
| ------ | ------- | ------ |
| P-value is less than your significance level (P < α) | the observed data is very unlikely under the assumption that the null hypothesis is true. Since the probability of observing such extreme results is low, we have sufficient evidence to reject the null hypothesis. | Rejecting the null hypothesis suggests that there is a statistically significant effect or relationship present in the data. |
| P-value is greater than your significance level (P > α) | indicates that the observed data is consistent with the null hypothesis. The probability of observing such results is relatively high under the null hypothesis, suggesting that we do not have enough evidence to reject it. | This does not prove that the null hypothesis is true; it simply indicates a lack of evidence against it |

### 6.3. One-tailed and two-tailed tests
| Test | Result | Symbol |
|-----|---------| --------|
| A one-tailed test | results when the alternative hypothesis states that the actual value of a population parameter is either less than or greater than the value in the null hypothesis. | "<" / ">" |
| Two-tailed test | results when the alternative hypothesis states that the actual value of the parameter does not equal the value in the null hypothesis | ~= |

### 6.4. A/B Testing



## 7. Regression Analysis
regression analysis is about estimating relationships between a single dependent variable and one or more independent variables.

The dependent variable is the variable a given model estimates. Sometimes the dependent variable is also called a response or outcome variable and is commonly represented with the letter y
We assume that the dependent variable tends to vary based on the values of independent variables, typically represented by an x. Independent variables are also referred to as explanatory variables or predictor variables.

Y = slope * x + intercept (when x = 0 ,the value of y)

Correlated = they have linear shape
Ordinacry Least Squares Estimation (One of the most common way)

| type|effect |
| ---- | --- |
| positive| increase and decrease together |
| negative| inverse |

### Linear regression equation

B_0 * (intercept) + B_1 (slope) * X
Beta are parameter (parameter is from peopulation and not from sample)

The only way for this is to estimate

^B_0 + ^B_1X = y

^B_1 is also called regression coefficients. It estimated betas in a regression model.

We also try to minimize the loss function. It is a function that measures the distance between observed values and the model's estimated values. (We try to find the best line instead of just finding a line)

### logistic regression (optional)

Logistic regression is a technique that **models a categorical variable based on one or more independent variables.**
- It is because some thing will be only true or false, not a line can model
- outcome variable can be catrgorical

The link function connects, or links, a dependent variable to the independent variables mathematically. Data professionals use the link function to express the relationship between the X’s and the probability that Y equals some outcome

**Correlation is not causation**

## Python Programming
1. Beginning
- .describe() convenient way to calculate many key stats all at once
    - if you want to pariticular check the value under the column, you can choose one column to explore more about it. 
*   `count`: Number of non-NA/null observations
*   `mean`: The arithmetic average
*   `std`: The standard deviation
*   `min`: The smallest (minimum) value
*   `25%`: The first quartile (25th percentile)
*   `50%`: The median (50th percentile) 
*   `75%`: The third quartile (75th percentile)
*   `max`: The largest (maximum) value
- .head() will give you the top rows of excel or csv file
- .shape() is used to understand data column and rows number
- range will not be provided by using .describe() as they do not provide range. You need to calculate it by using .max() - .min() 
- df.columns
- df.types
- pd.crosstab(df["Gender"], df["GenderGroup"]) # Find out the number of them who cross in table
- df.groupby(['Gender','GenderGroup']).size() # Used for quickly understand the data

    ```
    df = pd.read_excel('123.xlsx)
    df['Sells'].describe()
    df.head()
    df['Sells'].max() - df['Sells'].min() # Method to calculate range
    ```

2. Continuious data calculation
- df.hist() is used to make a quick histogram
- stats.zscore() is used to caculate the z-score
- We use .shape() to find out the numbers of rows and columns. The row is the first one in returned tuple and the column is the second one.
- .mean() for mean and .std() for sd
- stats.norm.cdf(0) # Calculate the prob of continuous distribution

    ```
    df = pd.read_excel('123.xlsx)
    # common way to find the mass of the continuous distribution. If you do not use mean , it only return some true or false outcome. Using .mean(), it will create better result.
    ((df['aqi_log'] >= x) & (df['aqi_log'] <= y)).mean()
    df [ (df['Z_SCORE']> 3) | (df['Z_SCORE'] < -3)]
    df['Z_SCORE'] = stats.zscore(df['aqi_log'])
    ```

3. Sample data calculation

```
# Sampling in python
sampled_data = education_districtwise.sample(n=50, replace=True, random_state=31208)
sampled_data.mean()

# Below is the test of sampling
estimate_list = []
for i in range(10000):
    estimate_list.append(education_districtwise['OVERALL_LI'].sample(n=50, replace=True).mean())
estimate_df = pd.DataFrame(data={'estimate': estimate_list})
```

- n: You're sampling from 50 districts, so your sample size is 50.
- replace: For the purpose of our example, you'll sample with replacement. True indicates sampling with replacement.
- random_state: Choose an arbitrary number for your random seed. Say, 31208.
- Simple visualization example

```
# How to create a hostogram in python
plt.hist(estimate_df['estimate'], bins=25, density=True, alpha=0.4, label = "histogram of sample means of 10000 random samples")
xmin, xmax = plt.xlim()
x = np.linspace(xmin, xmax, 100) # generate a grid of 100 values from xmin to xmax.
p = stats.norm.pdf(x, mean_sample_means, stats.tstd(estimate_df['estimate']))
plt.plot(x, p,'k', linewidth=2, label = 'normal curve from central limit theorem')
plt.axvline(x=population_mean, color='g', linestyle = 'solid', label = 'population mean')
plt.axvline(x=estimate1, color='r', linestyle = '--', label = 'sample mean of the first random sample')
plt.axvline(x=mean_sample_means, color='b', linestyle = ':', label = 'mean of sample means of 10000 random samples')
plt.title("Sampling distribution of sample mean")
plt.xlabel('sample mean')
plt.ylabel('density')
plt.legend(bbox_to_anchor=(1.04,1))
plt.show() 
```

4. Confidence interval calculation
If you’re working with a large sample size, say larger than 30, you can construct a confidence interval for the mean using `scipy.stats.norm.interval()`. This function includes the following arguments: 

*   `alpha`: The confidence level
*   `loc`: The sample mean
*   `scale`: The sample standard error

```
estimated_standard_error = sampled_data['OVERALL_LI'].std() / np.sqrt(sampled_data.shape[0])
stats.norm.interval(alpha=0.95, loc=sample_mean, scale=estimated_standard_error)
stats.norm.interval(alpha=0.99, loc=sample_mean, scale=estimated_standard_error)
```
    df = pd.read_excel('123.xlsx)
    # common way to find the mass of the continuous distribution. If you do not use mean , it only return some true or false outcome. Using .mean(), it will create better result.
    ((df['aqi_log'] >= x) & (df['aqi_log'] <= y)).mean()
    df [ (df['Z_SCORE']> 3) | (df['Z_SCORE'] < -3)]
    df['Z_SCORE'] = stats.zscore(df['aqi_log'])
    ```

4. Sample data calculation

```
# Sampling in python
sampled_data = education_districtwise.sample(n=50, replace=True, random_state=31208)
sampled_data.mean()

# Below is the test of sampling
estimate_list = []
for i in range(10000):
    estimate_list.append(education_districtwise['OVERALL_LI'].sample(n=50, replace=True).mean())
estimate_df = pd.DataFrame(data={'estimate': estimate_list})
```

- n: You're sampling from 50 districts, so your sample size is 50.
- replace: For the purpose of our example, you'll sample with replacement. True indicates sampling with replacement.
- random_state: Choose an arbitrary number for your random seed. Say, 31208.
- Simple visualization example

```
# How to create a hostogram in python
plt.hist(estimate_df['estimate'], bins=25, density=True, alpha=0.4, label = "histogram of sample means of 10000 random samples")
xmin, xmax = plt.xlim()
x = np.linspace(xmin, xmax, 100) # generate a grid of 100 values from xmin to xmax.
p = stats.norm.pdf(x, mean_sample_means, stats.tstd(estimate_df['estimate']))
plt.plot(x, p,'k', linewidth=2, label = 'normal curve from central limit theorem')
plt.axvline(x=population_mean, color='g', linestyle = 'solid', label = 'population mean')
plt.axvline(x=estimate1, color='r', linestyle = '--', label = 'sample mean of the first random sample')
plt.axvline(x=mean_sample_means, color='b', linestyle = ':', label = 'mean of sample means of 10000 random samples')
plt.title("Sampling distribution of sample mean")
plt.xlabel('sample mean')
plt.ylabel('density')
plt.legend(bbox_to_anchor=(1.04,1))
plt.show() 
```

| Example | Description |
| ----------- | ----------- |
| P(X = 4) in throwing a dice once | find the prob of throwing the value 4 |
| P(X = 4) in throwing two dice | Find the prob that two dice sum is 4 |
