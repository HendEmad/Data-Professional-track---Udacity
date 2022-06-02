We use it to find the assumption of something existance or not.

For example: if the packaging on a loght bulb states that the bulb will last 500 hours under normal use. A consumer advocate would like to know if the mean lifetime of a bulb is less than 500 hours! There are two assumptions in this case. this statement is true or false?

- for sure, we will not test each bulb, but we will take a sample data from them.
- We test these types of statements using sample data because it is usually impossible to gain access to the entire population. This procedure we use to test such statements is called ***Hypothesis Testing***. 

- `If population data are available, there is no need for inferential statistics!`

- The statement can be either true or false. So, the hypothesis testing is based in two types of hypotheses which are: Null hypothesis & alternative hypothesis.
    1. Null hypothesis: H0
        * No change, no effect.
        * It is assumed true until evidence indicates otherwise.
        * It is the condition we believe to be true before we collect any data.
        * Mathematically, It is a statement of equal two groups or an zero-effect.
        * It holds some sort of equal signs: =, ≤, ≥
    2. Alternative hypothesis: H1
        * It is a statement that we are trying to find evidence to support.
        * It is what we would like to prove to be true.
        * It holds: ≠, >, <
* The H0 and H1 are competing, non-overlapping hypotheses.

- There are three ways to setup the null and alternative hypotheses:
1. ***two-tailed test*** --> Equal hypothesis versus not equal hypothesis
    H0: parameter = some value
    H1: parameter ≠ some value
2. ***left-tailed test(One tailed test)*** --> Equal versus less than
    H0: parameter = some value
    H1: parameter 6 some value
3. ***right-tailed test(One tailed test)*** --> Equal versus greater than
    H0: parameter = some value
    H1: parameter 7 some value
    
`Example:` 

* In the US judicial system, we say "Innocent until proven guilty". So, every indicidual is either innocent or guilty of an act. SO, this statement refers that everyone is innocent initially --> This is `null hypothesis(H0)` --> This refers to the rule that "H0 is the condition we believe to be true before we collect any data."
* Gulity --> is the `alternative hypothesis(H1)` --> "The competing alternative hypothesis is that an individual is guilty"
* We then collect data to see which hypothesis is supported.

There are 4 posibilities of this example:

![Screenshot (544)](https://user-images.githubusercontent.com/91827137/171724699-7a6d256b-8ec3-47c6-bdf6-21b443be4698.png)

![Capture](https://user-images.githubusercontent.com/91827137/171724872-b1cc2efa-d312-425f-9985-c161960bd903.PNG)

According to this example:

There are two types of errors that are possible in hypothesis testing:
  * Type I Errors and Type II Errors.
    * `Type I Errors` are considered `the worst type of error`.
    * A `Type I Error` is when the `alternative` is chosen, but the `null` is actually `true`.
      [***Type I error*** occurrs if `H1 is chosen when H0 is true`], this is also called             ***False Positive*** ---> denoted by the symbol `α` or `alpha(Commonly these rates are 1-       5%.)` 
    * A `Type II Error` is when the `null hypothesis` is chosen and the altrernative is actually       true, this is also called ***False Negative*** ---> They are denoted by the symbol `β` or       `beta`.
    * SO:
      * α = P(Type I Error) = P(rejecting H0 when H0 is true)
      * β = P(Type II Error) = P(not rejecting H0 when H1 is true)

***Note***: Correctly setting up the null and alternative hypotheses is important for avoiding these two types of errors.

***Question***
Just based on this information, can you guess which truth/decision combo is for each type of error?
- Truth: Innocent, Decision: Guilty -----> Type I Error
- Truth: Guilty, Decision: Innocent -----> Type II Error
- Truth: Innocent, Decision: Innocent -----> No Error
- Truth: Guilty, Decision: Guilty -----> No Error

There are two extreme cases:
1. Always choosing the null hypothesis:
  * In this case, we may avoid Type I Error, but Type II Errors may be much.
2.  Always choosing the alternative hypothesis:
  * In this case, we may avoid Type II Error, but Type I Error may be much.

There is a Threshold for how many type I errors occurring, and then they try to keep the Type II Error as low as possible while still meeting this threshold.
- Type I Error rates are 0.01 for medical field, 0.05 for research and business.
