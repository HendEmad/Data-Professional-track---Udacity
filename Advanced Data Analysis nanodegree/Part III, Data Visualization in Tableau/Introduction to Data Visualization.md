## What visualization we use depends on two things: 
1. Date Type (Categorical: Ordinal(Ordered), Nominal) / Quantitative: Continuous, Discrete).
2. How many columns in the dataset we want to look at in a single plot. 

- If no.of column in One --> Univariate analysis(Uni stands for One).

## Plots used for Univariate QUANTITATIVE data (both continuous and discrete):
1. Histogram (The most common one).
2. Box and Whisker Plot.
3. Normal Quantile Plot.
4. Stem and Leaf Plot.

![33560553-f8cfd8b2-d907-11e7-92fe-6d7103b5426d](https://user-images.githubusercontent.com/91827137/163528359-7d9b6678-f328-4d4a-b781-01612d3bebe6.jpg)

## Plots used for Univariate Categorical data ( both nominal, ordinal):
1. Bar Chart ( The most common one):
It is like a histogram, but the bins are determined based on a set category not on a range. It makes more sense to use it while working with categorical ordinal variable.
2. Par Chart.
3. Pareto Chart: They are essentialy just bar charts where the bars are in the order from the most to the least frequent.
_note:_ In manufacturing companies, pareto charts are used all the time to determine which parts have the most problems.

![Capture](https://user-images.githubusercontent.com/91827137/163528979-ae7200e2-f302-4dbc-be71-47fe5d9ed31e.PNG)

## Quiz 1:
1. Consider we look at an entire library full of books. An example of our dataset is shown here:

![Capture](https://user-images.githubusercontent.com/91827137/163538066-f49cc98d-fb36-4951-be20-7c705e1de216.PNG)

I want to plot the number of books with a certain number of pages (or range of pages).

**_answer_**: This is a **_quantitative_** variable, so the best plot is **_Histogram_** and we can also use a **_Box-Plot_**, **_Stem-and-Leaf plot_** or **_normal quantile plot_**.

2. Now imagine we are selling cookies, and we are keeping track of how many each type are sold.

![Capture](https://user-images.githubusercontent.com/91827137/163538461-0997336b-f4ff-4aed-8cde-82e97ebcc547.PNG)

Which of the below are plots we could build to plot the number of each type of cookie sold? (Select all that apply).

**_Answer_**: This is a Categorical variable. So _**Pie Chart**_, _**Bar Chart**_, and _**Pareto Chart**_ can be used.

## Comparing Two Quantitative variables:
To compare any two quatitative variables as price&sales or heights&weights, we can use _**Scatter Plot**_. This is the most common plot in this case.

This plot can be used to visualize bioth the strength and the direction of the relationship between two variables.

![Screenshot (464)](https://user-images.githubusercontent.com/91827137/163539861-9751c706-ba11-4525-876e-c8f501ad1496.png)

- The strength (Strong / moderate / Weak) ---> This is determined with the spread of the points of the plot. As the points become more spread out from one another, the relation ship become weaker and vise versa. We aren't so much looking at the slope associated with the relationship as the spread can be constant while the slope increasing or decreasing.
- The direction (Positive / Negative) ---> This is determined by whether this spread is increasing or decreasing with another variable. In positive relationship, As one variable increases the other variable also increases. In negative relaionship, As one variable increases the other variable decreases.

![OIP](https://user-images.githubusercontent.com/91827137/163541754-9424d2a5-b6d1-41ca-ba9c-4c836f7d7dcf.jpeg)

- There is a numeric value used to capture these two aspects (Strenght and direction) is called the _**correlation Coefficient ( r )**_.

- This is used to find the stenght and the direction of a _**linear**_ relationship.
- It is always between -1 and 1, where the closer it is to 1 or -1, the stronger the relationship. The negative tells us that there's a negative relationship, while the positive tells us there's a positive relationship.

![Screenshot (466)](https://user-images.githubusercontent.com/91827137/163551004-e05dcab5-b4b1-4fe8-91cf-2b62ed9f74bf.png)

- A negative correlation coefficient is not indicative of a weak relationship. This means that even if we calaulated r, we still need to visualize the relationship.

***A rule of thumb for judging the **_strength_**:***
![Capture](https://user-images.githubusercontent.com/91827137/163551799-c44ef833-7155-49a0-8162-ccf7c7e07375.PNG)

***Calculation of the Correlation Coefficient***
![Capture](https://user-images.githubusercontent.com/91827137/163552187-c4ce55a7-b2be-4c3c-8373-2d337b5b4876.PNG)

- It can be calculated in Excel --> CORREL(col1, col2) where col1 and col2 are the two columns to compare to one another. The order of col1 and col2 doesn't matter here.

- correlation coefficient (Pearson's correlation) is only for measuring linear relationships.
- A correlation coefficient of 0 doesn't necessarily mean that there is no relationship between two variables. Rather that there isn't a linear relationship.

### Quantitative variable overtime visualization
Line plots are a common plot for viewing data over time. These plots allow us to quickly identify overall trends, seasonal occurrences, peaks, and valleys in the data. You will commonly see these used in looking at stock prices over time, but really tracking anything over time can be easily viewed using these plots.

## The key to building great data visualizations is in aiming them at answering the questions you want answered:

consider we run a blog, and we want ti understand traffic on thr blog. for simplicity, consider we just use 12 months worth of traffic:
- If we want to know the month we had the most traffic, the best plot would be a bar chart or pareto chart(as tbis would plot the months in order from heighest to lowest traffic). Here, each bar is the amount of traffic for a particular month.

![Screenshot (469)](https://user-images.githubusercontent.com/91827137/163555946-e537187f-e1f4-4351-910d-0e1bf665184b.png)

from the plot, we can easily notify that November had the heighest amount of traffic. 
- If we want to know if traffic was increasing over time, the best chart here would be the line chart.

![Screenshot (472)](https://user-images.githubusercontent.com/91827137/163556285-9d0b5aa8-8990-4b8c-9530-b3e80f210a0d.png)

This plot akso assests to know if a particular months had higher or lower traffic than other. 
May be September would always be a low, and November be higher than the other months in the year. 

Now, what if we had a multiple years worth of data and we want to know what the distribtution of the number of visitors looked like:
- How frequency were there more than 2000 visitors per month?
- What was the most common amount of visitors?

This would be to tough to be answered using the bar chart or the line chart. It's better to use the histogram to understand the typicak no.of visitorrs in a month. The height of the bars tells us how often a certain number of visitors has occurred.

![Screenshot (474)](https://user-images.githubusercontent.com/91827137/163557362-488b992d-8fa3-4477-9353-353733886259.png)

## Dealing with more than Two variables
***If we want to compare two categorical variables with another variable, we would probably use a **_Side by side bar chart.
![Screenshot (476)](https://user-images.githubusercontent.com/91827137/163563496-44722494-40eb-489b-9d46-4539d64a87f9.png)

for example, this plot shows the grouping for one category are grouped in color for the other variable. Using this, we can quickly identify the favourite flavor in each location.

- Other examples:
1. Line Chart of three variables which are sales, products, and time

![Screenshot (478)](https://user-images.githubusercontent.com/91827137/163563843-404f56b4-beb2-42f4-a34c-0e9fadcfa957.png)

2. Stacked line chart of three variables which are sales, products, and time

![Screenshot (480)](https://user-images.githubusercontent.com/91827137/163563995-50365a20-80e4-4ba5-8dd4-19d4647f2456.png)

This seems to be as the line chart, but here each product is shown in terms of proportion of the toal sales.

3. Stack bar chart:

![Screenshot (482)](https://user-images.githubusercontent.com/91827137/163564145-cbce4d7b-509c-44e4-bd99-aeaf1b2733e5.png)

Here, each product has a color in the bar, and the height of the bar is the amount of sales for each product.

## Quiz 4:

For these plots:

![screen-shot-2017-08-28-at-4 28 43-pm](https://user-images.githubusercontent.com/91827137/163564667-082c99c0-bf98-42d1-bfeb-f8a65e0e2e0f.png)

***Which product had the fastest growth in sales from January to July?***
- The answer is Product3, it is easiest to see in Plot 4.

***In which month did Product 1 have more than 50% of the sales?***
- The answer is February, this is easiest to see in Plot 1.

***Did total sales ever exceed 1000 units?***
- The answer is Yes, in November. this is easiest to see in either Plot 2 or Plot 3.

## Dashbords:

Sometimes a single plot cannot convey all the information in a data set. for example, if we want to compare price by sales by location and by the product, and then additionaly we want to see how these changes happen over time. In this case we will use data dashboards.

for example:
![Capture](https://user-images.githubusercontent.com/91827137/163566552-1deab859-c731-494c-916c-66df00aed277.PNG)

This is an example of data dashboards of Hans Rosling for 200 countries over 200 years!
Here, the dashboeard elements are:
- X-axis --> Income
- Y-axis --> Life Span
- Size of each circle --> Population
- Color of each circle --> Countries
-  Movement of the dashboard --> Time
-  The base blot used is --> Scatter Plot

The different colors and sizes are known as Visual Encodings. So this represents the way our variables in a plot. Each of the elements is a design component for the visual.
