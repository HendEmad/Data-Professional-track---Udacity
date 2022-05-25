## Descriptive vs. Inferential Statistics
***Descriptive Statistics*** :describing collected data.

***Inferential Statistics*** :Drawing conclusions about a population of individuals baesd only on a ```sample``` of individuals from that population.

## sampling distribution
the distribution of a statistic.

### Quiz
1. The mean of the sampling distribution ----> P
2. The variance of the original 1,0 values ----> P(1-P)
3. The variance of the proportions calculated from 20 randomly selected values iterated 10,000 times ----> P(1-P)/20

### Notes
- The sampling distribution is centered on the original parameter value.
- The sampling distribution decreases its variance depending on the sample size used. Specifically, the variance of the sampling distribution is equal to the variance of the original data divided by the sample size used. This is always true for the variance of a sample mean!
- In notation, we say if we have a random variable, **X**, with variance of **σ^2** , then the distribution X` (the sampling distribution of the sample mean) has a variance of **(σ^2) / n** 

* All parameters pertain to a population, while all statistics pertain to a sample.
* we commonly use Greek symbols as parameters and lowercase letters as the corresponding statistics. Sometimes in the literature, you might also see the same Greek symbols with a "hat" to represent that this is an estimate of the corresponding parameter.

![Capture](https://user-images.githubusercontent.com/91827137/168033978-4764dd4b-636c-4e39-83e6-29903943d62d.PNG)

# Two important mathematical theorems for working with sampling distributions
1. Law of Large Numbers ---> if we choose the right statistics to estimate a parameter. the larger out sample size, the closer out statistic gets to the parameter.
- The Law of Large Numbers says that as our sample size increases, the sample mean gets closer to the population's mean.

3. [Central Limit Theorem](https://medium.com/analytics-vidhya/understanding-the-central-limit-theorem-for-data-science-78f11544bbc6)
It states that with a large enough sample size, the sampling distribution of the mean will be normally distributed.

- The Central Limit Theorem actually applies to these well-known statistics:
1. Sample means (x`)
2. Sample proportions (p)
3. Difference in sample means (x1` - x2`)
4. Difference in sample proportions (p1 - p2)

# BootStrapping
Bootstrapping is sampling with replacement. Using random.choice in Python actually samples in this way. Where the probability of any number in our set stays the same regardless of how many times it has been chosen. Flipping a coin and rolling a die is like bootstrap sampling as well, as rolling a 6 in one scenario doesn't mean that 6 is less likely later.

# Recap Quiz
- A numeric summary of a sample. ---> Statistic
- A numeric summary of a population. ---> Parameter
- The distribution of a statistic. ---> Sampling Distribution
- Used to notate parameters. ---> Greek symbols
- Sampling with replacement. ---> BootStrapping

- A theorem that states: the larger the sample size, the closer our statistic gets to the parameter. ---> Law of Large numbers theorem
- A theorem that states: if our sample size is large enough, the sample mean will be normally distributed. ---> The central limit theorem
- Describing the data we have collected. ---> Descriptive Statistics
- Using the data we have collected to draw conclusions about our population of interest. ---> Inferential Statistics
