# Gramener Case Study

This study aims to explore a comprehensive loan dataset from Lending Club and derive insights from the same with the objective to narrow 
down on top drivers of bad loans.

Lending Club is the world's largest peer-to-peer lending platform. They offers lending service by connecting the borrowers with investors 
through an online marketplace. While this has became a popular source of passive income for investors, there is also risk of default, in which the 
borrowers fall behind on their repayments. In this study we use real market data from Lending Club to analyse over 39k loan transactions in the 
US along with numerous attributes and try to formulate a data backed approach to identify top drivers of bad loans. This could be used as 
features in models for risk assessment.

Our approach to solving this problem is quite simple and straight-forward. We pre process the data to get rid of redundant variables and 
features and then use univariate, segmented univariate and bi-variate analysis to identify variable distributions and patterns, We also study the 
dependency between set of two variables to find opportunities of correlating features that can predict risk.

Using this approach we finally narrow down on a set of features that can help us predict the probability of a loan going bad and hence 
minimising the risk for the lender.

# Results

From the above analysis, we can conclude that- following are the variables which can be used to identify the defaulters:

### Number of loan inquries in last 6 months (inq_last_6mths):
Default rate increases significantly as the number of inquires increases. If number of inquires are more than 2 then change of loan being a bad loan are substantially high.

### Number of derogatory records(pub_rec):
if a person has a public derogatory record then the change of him defaulting is significantly higher

### DTI:
The higher the dti the higher is the percentage of bad loans. But the difference with in dti range is not very high.

### Delinquency in last 2 years:
The person who has delinquent at least once in last 2 years has more chances being a defaulter again, but the difference in percentage between ‘No’ and ‘Yes – is delinquent is not very high.

### Number of open credit files:
We saw that open accounts less than 6 or more then 21 causes a higher percentage of loans to be defaulted.

### Loan amount:
We saw clearly saw a trend that as loan amount increases the tendency of defaulting a loan also increases. This is partly also because of having higher interest rates as we move down the grades.

### Annual income:

income decreases the tendency to default a loan increases.

### Purpose:
majority of loans are for purpose debt_consolidation. the default percentage is highest for small businesses which is about(25%).
