# Task
1. Explore the data and evaluate univariate relationship between the target variable and the individual predictor variables
2. Develop a model to predict which clients will be defaulted
3. Develop an application credit scorecard

# Method
- Use Python library (pandas, seaborn, matplotlib) to visualize data exploration
- Use Python library (sklearn) to predict default clients

# Result
**1. Explore the data**
According to the EDA:
- People finishes lower secondary has higher risk compared to other types of education
- Customers who living with their parents or renting apartment tend to default
- Low skills laborers, cooking staff and waiters tend to have higher risk than other occupation

**2. Develop a model to predict which clients will be defaulted**
_Interpret the model_
- Lower secondary education, occupation type 2 (cooking staff, security staff, barmen staff, realty agents, low-skill laborers, drivers, hr staff, secretaries) clients have a higher probability of default
- The larger the EXT2, EXT1, the less likely that the clients will default
- Clients with income type 4 (working, commercial associate) have lower probability to default
- Clients who did not specify the EXT1 and EXT3 variables tend to not default
- The longer the changing days of registration before application, the lower the probability that he/she will default

**3. Develop an application credit scorecard**
The scores of the customers are divided into 4 categories:
- Poor: 600 - 760
- Fair: 760 - 820
- Good: 820 - 850
- Excellent: 850 - 1000
