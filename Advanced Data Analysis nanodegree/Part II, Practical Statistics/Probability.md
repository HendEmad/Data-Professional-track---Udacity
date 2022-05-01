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

### Conditional probability theory → 
EX1) If we have three possibilities:
1. P(C) → Probability of cancer → p1
2. P(POS | C) → Probability of a positive test for someone who has cancer → p1
3. P(NEG | !C) → Probability of a negative test for someone who does not have cancer → P2

![Capture](https://user-images.githubusercontent.com/91827137/166150985-bc9839c4-8acf-46cd-8c62-be682e5f3703.PNG)

What this table represents is that 10% of the general population has cancer. 90% of people who have cancer, will test positive for cancer. And 80% of people who don't have cancer, will test negative for cancer.

The question is: What is the probability of getting a positive test for cancer for anyone in the general population given the data above regardless of the fact they have cancer or not?
- By logic, people who test positive regardless of having cancer or not = 
(People who have cancer and test positive)  or (people who don’t have cancer and test positive.

People who have cancer → P(C), People who have cancer, test positive → P(POS|C),
People who don’t have cancer → P(!C) = 1 - P(C),
People who don’t have cancer, test positive → P( POS|!C) = 1 - P(NEG|!C)

- So, the answer will be: 
P(POS) = P(C) * P(POS| C) + P( C) * P(POS|  C) → This is a mathematical notation called Total Probability
              = P(C) * P(POS| C) + (1 - P(C)) * (1 - P(NEG| C))
              = 0.1 * 0.9 + (1 - 0.1) * (1 - 0.8) = 0.27 
              
EX2) A person can either have cancer or not have cancer: 

P(Cancer) = 0.1, 
P(!Cancer) = 0.9

- In this example, 10% of people have cancer and therefore 90% of people do not.
Conditional Probability: Having cancer might be determined with a test. We now are working with Conditional Probabilities. A test result could be positive or negative and a person could or could not have cancer.

Example: P(Positive|Cancer) = 0.9
- In the case above the probability of a positive test, given someone does have cancer is 0.9 or 90%. The pipe/bar “|” character denotes the outcome of the first condition depends on the second condition.

The second value depends on the existence or non-existence of the first value which means:

P(negative | cancer) = 1 - P(positive | cancer) 

Thr first value which is (positive or negative) depends on the cancer existence. then in case of cancer non-existence, the values will be different. They are two different cases.

Also → P(negative | cancer) = 1 - P(positive | cancer) 

Table of the Cases:

![Capture](https://user-images.githubusercontent.com/91827137/166152864-be9ccfad-c6ff-47ea-8726-0e8bb73852e0.PNG)

So, P(negative |  cancer) = 1 - P(positive |  cancer) = 1 - 0.2 = 0.8

Aimed with the information from above we can start building out a Truth Table for these cases that looks like this:

![Capture](https://user-images.githubusercontent.com/91827137/166152885-f62709ed-0fa5-43b0-a8d9-2d2fadecb305.PNG)

The question is: What is the probability of Case 1 from the table above where a person has cancer and tests positive for cancer?

The answer is 0.09
- By multiplying P(cancer) * P(positive | cancer) 
--> “HAVE CANCER AND TESTS POSITIVE” = HAVE CANCER AND (HAVE CANCER & POSITIVE) = 0.1 * 0.9 = 0.09


OR  The probability of cancer 0.1 times the probability of testing positive and having cancer 0.9.

We will complete the table in the same way for all 3 remain cases and the results will be:

![Capture](https://user-images.githubusercontent.com/91827137/166152966-92fbfef8-c10a-49bc-9411-29dd2082c89e.PNG)

***NOTE*** : Sum of the probabilities = 1 (must always be 1)

Another question here: What is the probability of someone testing positive for cancer given the information above?

Answer → We just need to look at where the tests were positive and sum the values.
                  = 0.09 + 0.18 = 0.27

Another example — Two coins
We are now placing two coins in a bag.
          Coin 1 is a fair coin --> P1(H) = 0.5
          Coin 2 is a loaded coin --> P2(H) = 0.9

What is the probability of tails for each coin given the information above?

P1(T) = 0.5 (1 - 0.5)

P2(T) = 0.1(1 - 0.9)

Now we want to figure out what the probability of getting heads or tails would be when pulling a random coin from our bag. There are two coins so there are equal chances that we could pull either one.

P(1) = 0.5, P(2) = 0.5. What we know so far:

![Capture](https://user-images.githubusercontent.com/91827137/166153070-be094dce-79db-406f-abe1-2a86e3438e10.PNG)

What is the probability of flipping Heads when pulling a random coin from the bag?

Solution → P = P(1) * P1(H) + P(2) * P2(H) = 0.5 * 0.5 + 0.5 * 0.45 = 0.7

Next, we want to pick one coin from the bag and flip that coin two times. Truth table is:

![Capture](https://user-images.githubusercontent.com/91827137/166153117-fa281db1-23d1-4b77-b6b0-dd3fddea5d23.PNG)

Once we know those probabilities, we can sum them to find our answer:
0.125 + 0.045 = 0.17

We again want to pick one coin from the bag and flip that coin two times. However this time both coins are loaded. P(H|1) = 1, P(H|2) = 0.6

![Capture](https://user-images.githubusercontent.com/91827137/166153166-477f017c-dfbe-4b0f-af25-47c1642eb937.PNG)

If we sum both cases, 0.0 + 0.08 = 0.08 which is the answer
