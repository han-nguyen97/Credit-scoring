# Task
1. Explore the data and evaluate univariate relationship between the target variable and the individual predictor variables
2. Develop a model to predict which clients will be defaulted
3. Develop an application credit scorecard

# Method
- Use Python library (pandas, seaborn, matplotlib) to visualize data exploration
- Use Python library (sklearn) to predict default clients

# Result
**1. Explore the data** <br\>
According to the EDA: <br\>
_The relation between numerical variables and target variable:_
- Default customers have slightly lower income compared to non-default customers
- The loan amount of default customers is lower than the non-default customers
- There is no difference in terms of duration in loan between non-default and default clients  
- Young people tend to present more risk than the older ones
In general, older people usually have more financial stability than the younger ones;
From the perspective of a bank or a loan establishment, probably it's safer to offer better credit programs to people who has the condition to pay back.
- People with shorter employment days have higher tendency to be default
The number of working days may correlate with the financial situation of a customer. The higher the number of employment days, the more solid the financial stability. As a result, customers with lower job experience may have a higher risk than those with higher employment days 
- Shorter registration days related to a higher risk
- The shorter the number of days to change phones before using the application, the higher the risk

  _The relation between categorical variables and target variable:_
- People who finish lower secondary have higher risk compared to other types of education
- Customers who live with their parents or rent an apartment tend to default
- Low-skilled laborers, cooking staff and waiters tend to have a higher risk than other occupation

**2. Develop a model to predict which clients will be defaulted**
_Interpret the model_
- Lower secondary education, occupation type 2 (cooking staff, security staff, barmen staff, realty agents, low-skill laborers, drivers, hr staff, secretaries) clients have a higher probability of default
- The larger the EXT2, EXT1, the less likely that the clients will default
- Clients with income type 4 (working, commercial associate) have a lower probability of default
- Clients who did not specify the EXT1 and EXT3 variables tend to not default
- The longer the changing days of registration before application, the lower the probability that he/she will default

**3. Develop an application credit scorecard**
The scores of the customers are divided into 4 categories:
- Poor: 600 - 760
- Fair: 760 - 820
- Good: 820 - 850
- Excellent: 850 - 1000
