# Probability:
- In probability, we make predictions about the future events based on causes that we assume (You predicting data).
- In Statistics, we analyze the data from the past events to infer (understand) what those causes could be (You are using the data to predict). 
- The probability of a fair coin notation is — P(Heads) = 0.5.
- Probability Law — P(Heads) + P(Tails) = 1
- The formula applies to anything that has only two outcomes — P(Outcome 1) + P(Outcome 2) will always equal 1

***note*** (Fair coin is one whose two parts have the same frequency to appear)

- Probability Formula — The probability of P (A) = 1− P (¬A).

--> This reads the probability of A = 1 minus the probability of not A.

- Probability is a number between 0 and 1
- Truth Table size for coin flips is determined by the number of sides (Head/Tail) with an exponent equal to the number of flips. So 10 flips of a coin would have a Truth Table size of 
210  or 1024.

![Capture](https://user-images.githubusercontent.com/91827137/165458728-d1cf8950-4b61-44be-9d45-aa020068be8c.PNG)

--> So, P(H, H) = P(H, T) = P(T, H) = P(T, T) = 0.25 — in fair coins.
Another way to calculate this → P(H, H) = P(H) * P(H) = 0.5 * 0.5 = 0.25

→ If we flipped the fair coin twice, there are two cases where we can see heads once which are (H, T) & (T, H) – Here, the head appears only one time in each case. So, to figure out the probability of heads coming up just once, we add the probabilities together: 
P(H) = P(H, T) + P(T, H) = 0.25 + 0.25 = 0.5

→ Rolling 1 Heads in Three Flips: 

![Capture](https://user-images.githubusercontent.com/91827137/165459029-8297ad2a-e532-4c7d-81ff-6c0a28efd555.PNG)

--> Because there are eight possibilities and they each could occur with the same probability which is 1/8 or 0.125. Further, only Cases 4, 6, and 7 have the possibility of having only one Head. If you sum them, you get 0.375 (0.125 + 0.125 + 0.125 = 0.375).

--> ***If the coin is loaded and P(H) = 0.6. So, we will use the multiplication method: ***

```Q)``` What is the probability of seeing only one Head in three flips with a loaded coin? P(H) = 0.6

```Answer``` P(H) = 0.6 → → → P(T) = 0.4

-> H will appear once in three cases so H * H * H = 0.6 * 0.6 * 0.6 = 0.288 OR (0.6 * 0.4 * 0.4) * 3 = 0.288

***Note***
Probability rules are used when trying to figure out only independent variables.
So, If we are trying to figure out the probability of dependent events, like what is the probability that it will rain tomorrow if it rained today, do not follow these same rules.

# Binomial Distribution
- Determines the probability of a string of independent coin flip-like events.
- Number of Ways to get k Heads in n flips of a coin: ```n! / k! * (n-k)!```
- Probability of k Heads and (n-k) Tails: ```(p^k) * ((1-p)^(n-k))```
-  Binomial Distribution Formula: ```n! / (k! * (n-k)!) * (p^k) * ((1-p)^(n-k))``` 

# Practical Statistics:

Conditional Probability: The probability of the outcome of one event is affected by the outcome of another event.










