# Bank — Customer Churn Analysis

## Used tools: 
* `pandas`
* `matplotlib`
* `seaborn`
* `numpy`
* `scipy`
* `plotly`

## Project description

**Client** - regional bank "Metanprom”

The client has access to a dataset with anonymized user data.

**Dataset Columns:**
* `USERID `- user identifier
* `city` - city
* `score` - credit scoring points
* `gender` - gender
* `age` - age,
* `equity` - number of owned objects
* `balance` - account balance
* `products` - number of products used by the client
* `credit_card` - presence of a credit card (yes/no)
* `last_activity` - active client (yes/no)
* `EST_SALARY` - estimated salary of the client
* `churn` - churn status (whether the client left or not)

## Task description

**Task:** Conduct an analysis of customers of the regional bank and **identify segments** (profiles of groups defined by 2-3 features) of customers who are prone to churn from the bank's services.

**Results:** Prepare a presentation and dashboard that can demonstrate the research findings effectively.

## Overall conclusion
**As a result of in-depth (exploratory) data analysis, the following observations have been made:**

1. The churn rate is higher for males compared to females.
2. The highest churn occurs in the Yaroslavl branch, while the lowest is in Rybinsk.
3. Most churn is among customers without credit cards.
4. Inactive customers are less likely to churn.
5. Customers with ownership scores of 3 or higher are more likely to churn. Over 50% of clients with a property score of 9 are inclined to leave.
6. Customers with more than 3 products are prone to churn.
7. Customers with credit scores between 830 and 900 are prone to churn.
8. Two client age groups are prone to churn: 25–35 years old and 50–60 years old.
9. Clients tend to churn when their balance is 700 thousand or more.
10. Clients with high salaries, over 100 thousand, are more likely to churn.

**Based on the results of the exploratory data analysis, the following segments with the highest churn rates were identified:**

**First Segment:** 	
- clients with good credit score 830-900
- clients without a credit card
- active clients

**Second Segment:** 
* clients over 50 years old
* male clients
* clients with property points above three

**Third Segment:** 
* young clients 25-35 years old
* clients with good credit score 830-900
* clients who have a credit card
* active clients

## Materials

* [Dashboard](https://public.tableau.com/app/profile/natalia.zvereva/viz/_16938672598280/sheet1)
* [Presentation](https://docs.google.com/presentation/d/1W4GetguhFQclC6S0341AQju2JuNPbk0lrixbSwGb2Ps/edit?usp=sharing)
