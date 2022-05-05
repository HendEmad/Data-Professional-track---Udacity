### Quiz 1: Robot Sensing1:
Imagine a robot that lives in exactly two places – red place (R) and green place (G). Initially, the robot can not tell where it is so—
- P(R) = P(G) = 0.5.

The robot has unreliable visual sensors—
- Probability of seeing red when in red is P(see R | at R) = 0.8
- Probability of seeing green when in green is P(see G | at G) = 0.8

What are the posterior probabilities of being at a red place given that the robot sees red and not having being in a red place given seeing red?

So:

- P(SEE G|AT R) = 1 - P(SEE R|AT R) = 1 . 0.8 = 0.2
- P(SEE R|AT G) = 1 - P(SEE G|AT G) = 1 - 0.8 = 0.2

-------------------------------------------------------------------------------

- AT R hypothesis = P(AT R, SEE R) = P(R) * P(SEE R|AT R) = 0.5 * 0.8 = 0.4
- AT G hypothesis = P(AT G, SEE R) = P(G) * P(SEE R|AT G) = 0.5 * 0.2 = 0.1
- P(SEE R) = Normalizer = P(AT R, SEE R) + P(AT G, SEE R) = 0.4 + 0.1 = 0.5
- posterior probability (AT R) = P(AT R|SEE R) = P(AT R, SEE R) / P(SEE R) = 0.4 / 0.5 = 0.8
- posterior probability (AT G) = P(AT G|SEE R) = P(AT G, SEE R) / P(SEE R) = 0.1 / 0.5 = 0.2

-------------------------------------------------------------------------------------------------

### Quiz 2: Robot Sensing 2:
The robot still lives in exactly two places – red place (R) and green place (G), but now:
- P(R) = 0
- P(G) = 1

The robot has unreliable visual sensors—
- Probability of seeing red when in red is P(see R | at R) = 0.8
- Probability of seeing green when in green is P(see G | at G) = 0.8

What are the posterior probabilities of being at a red place given that the robot sees red and not having being in a red place given seeing red?

SO:

- P(SEE G|AT R) = 1 - P(SEE R|AT R) = 1 - 0.8 = 0.2
- P(SEE R|AT G) = 1 - P(SEE G|AT G) = 1 - 0.8 = 0.2

-----------------------------------------------------------------------------

- P(AT R, SEE R) = P(R) * P(SEE R|AT R) = 0 * 0.8 = 0
- P(AT G|SEE R) = P(G) * P(SEE R|AT G) = 1 * 0.2 = 0.2
- P(SEE R) = 0.8 + 0.2 = 0.2
- P(AT R|SEE R) = P(AT R, SEE R) / P(SEE R) = 0 / 0.2 = 0
- P(AT G|SEE R) = P(AT G|SEE R) / P(SEE R) = 0.2 / 0.2 = 1

----------------------------------------------------------------------------------------------

### Quiz 3: 
Now we have a robot that lives in exactly three places – red place (A), green place (B), and green place (C). Initially, the robot can not tell where it is so—
- P(A) = P(B) = P(C)= 1 / 3 =0.333

The robot has unreliable visual sensors—
- Probability of seeing red when at A is P(see R| at A) = 0.9 --> 
- Probability of seeing green when at B is P(see G | at B) = 0.9 --> P(SEE R|AT B) = 0.1
- Probability of seeing green when at C is P(see G | at C) = 0.9 --> P(SEE R|AT C) = 0.1

1. What is the joint probability of being at A given that the robot sees red, P(A, R)?
- P(A, R) = P(A) * P(R|A) = 0.333 * 0.9 = 0.3
2. What is the joint probability of being at A given that the robot sees red, P(B, R)?
- P(B, R) = P(B) * P(R|B) = 0.333 * 0.1 = 0.0333
3. What is the joint probability of being at A given that the robot sees red, P(C, R)?
- P(C, R) = P(C) * P(R|C) = 0.333 * 0.1 = 0.0333
4. What is the normalizer for this example?
- P(R) = 0.3 + 0.033 + 0.033 = 0.3666
5. What are the posterior probabilities for all three possibilities, given that the robot sees red?
- P(AT A|SEE R) = P(A, R) / P(R) = 0.3 / 0.3666 = 0.818
- P(at B|see R) = P(B, R) / P(R) = 0.0333 / 0.3666 = 0.091
- P(at C|see R) = P(C, R) / P(R) = 0.0333 / 0.3666 = 0.091

_NOTE HERE_ : Unsurprisingly, the sum of the posterior probabilities is 1.

_NOTE_ : Bayes Rule can be applied to very large problems, with many possible hidden causes, but the mathematical calculations still remain true.

### Quiz 4: Sebastian At Home
These are the facts given—
-Probability Sebastian is not home – P(gone) = 0.6
- Probability Sebastian is home – P(home) = 0.4
- Probability of seeing rain when at home – P(rain|home) = 0.01
- Probability of seeing rain when not at home – P(rain|gone) = 0.3

What is the probability that Sebastian is home, given that he sees rain, P(home| rain)?
- (P(home)⋅P(rain ∣ home)) / (P(home)⋅P(rain ∣ home) + P(gone)⋅(1 − P(rain ∣ gone))) = (0.4 * 0.01) / (0.4 * 0.01 + 0.6 + 0.3) = 0.0217
