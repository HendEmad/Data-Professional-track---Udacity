- All of testing and confidence intervals are defined through the normal distribution; because in most of experiments, we foten have a huge number of data points.

- You flip a fair coin 1000 times in an experiment. The mean value of # heads divided by 1000 is approximately the probability of getting head when flipping a coin, which is 0.5. If you do this experiment 1000 times, what is the shape of the distribution of the mean value?
 
 ![Capture](https://user-images.githubusercontent.com/91827137/167325756-ee4768ab-5ce1-435e-94ac-95796913bbc8.PNG)

![2](https://user-images.githubusercontent.com/91827137/167325771-9cb19b66-cd86-44f2-9837-d3cad5ee2a00.PNG)

![Capture](https://user-images.githubusercontent.com/91827137/167329006-c88aa688-8902-4414-bb86-91eb1986755f.PNG)

This distribution describes the limit of computing a mean over any set of experiments, which means that no matter what kind of experiment you do, as long as you do it a large number of times, the mean of the experiment results will always have a distribution like this.

However, there is one flaw of this distribution - the area under the curve adds up to sqrt(2πσ), which is not very intuitive to study statistics and probability because the probability always adds up to 1. So the true normal distribution is normalized by 1 / sqrt(2πσ). The normal distribution can be written as:
![Capture](https://user-images.githubusercontent.com/91827137/167329426-adab6a6d-a41e-449b-b7fa-055f8eac95ff.PNG)

where μ is the mean and σ ^ 2 is the variance of the normal distribution.
