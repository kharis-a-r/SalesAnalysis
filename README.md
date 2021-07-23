# Sales Analysis
Check out the ipynb files
---
This is an analysis of sales data from a chainstore for Year 2019.
The analysis **gain insight of the sales pattern** and also aim to answer some questions in order to **improve sales** of said chainstore by applying best strategies generated from the data. <br><br>

---
Steps of the analysis explained below:<br>
### 1. Load and merge data
The raw data consists of 12 files in csv format and thus should merged first into a dataframe.

### 2. Clean up the data
Initial step to analysis a data is to clean up the data, mostly:
- transform NaN values (drop or replace with median)
- adjust data types to it's suitable types
- add some feature column (extract states from address, extract month from date, etc)

### 3. Exploratory Data Analysis
This is the main step from the analysis of a data. We try to answer some question to set the strategies to improve sales from data.
#### Question 1: What was the best month for sales? How much was earned that month?
To answer the question, I have to generate total sales (in $) since the original data doesn't have the total sales column. Then I group total sales based on month and make a graph out of it.<br><br>
The answer to this question set the strategies to put resources to maximize sales in certain months where sales peak.
#### Question 2: What city sold the most product?
To answer this question, I have to make a new column "City" because the original dataframe doesn't have specific City column. I then group total product and total sales based on city. <br><br>
The answer to this question set the strategies to put more advertisements in targeted city
#### Question 3: What time should we display advertisemens to maximize the likelihood of customer’s buying product?
This is a timeframe analysis and grouping total sales based on hour it's purchased.
#### Question 4: What products are most often sold together?
This is an interesting problem since we have to group products sold by order ID and then count the most two products sold together.<br><br>
We can set the strategies to advertise these two products (i.e to give promo if these 2 purchased together) to increase sales
#### Question 5: What product sold the most? Why do you think it sold the most?
This is to find out why some product sell better then the others and thus we can maximize sales of the products that already sell best and set different strategies especially for expensive products but doesn't sell much.
