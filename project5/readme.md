# Prosper Loans Data Exploration

## Dataset

The data consists of information regarding more than 100,000 loans on Prosper with more than 80 features.
The dataset can be found [here](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1608053448414000&usg=AOvVaw3QHm2jzSaCPaBUbEvUXtSg),
with feature documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).

## Wrangled Dataset

We have selected some features of interest from the available 81 features, performed data cleaning to remove duplicates,
missing values, and make the data more consistent for analysis. These changes were saved to a new dataset `prosper_loan_sub.csv`,
which is attached along other project files.

## Summary of Findings

In the process of exploring the dataset, we have found a strong positive relationship between
the interest rate and the annual percentage rate. Both the interest rate and the annual 
percentage rate tend to follow an approximatelly normal distribution. Another strong positive
relationship was found between both loan original amount and monthly loan payment. Both the
original loan amount and the monthly loan payment tend to follow a right-skewed distribution.
A moderately negative relationship was found between the interest rate and original loan amount.
Non-completed loans were associated with higher interest rates and higher loan original amounts,
when compared separately. A linear relationship was found between the interest rate and prosper
rating, with higher risk ratings associated with higher interest rates. Analyzing the interaction
between the interest rates and original loan amount across different loan outcomes, we found that
non-completed loans were more associated with lower loan amounts and higher interest rates.
Analyzing the interaction between the interest rates and original loan amount across different 
prosper ratings, we found that higher risk ratings were more associated with lower loan amounts 
and higher interest rates. Non-completed loans and higher risk ratings are both associated with
lower loan amounts and higher interest rates.

Several other features were explored. Some features such as number of recommendations, employment status,
and verifiable income, did not have much variety for a meaningful analysis. Other features such as
homeownership and loan term were also explored. we have found that homeowners are more associated with
higher loan amounts and lower interest rates. We also found that he most frequent loan term chosen by
borrowers is 36 months (3 years). 60 months (5 years) term is the second more common and a term of 
12 months (1 year) is chosen by a very few proportion of borrowers.

## Summary of  The Presentation

The presentation will focus on our main features of interest. We will start by showing the count of the
different loan outcomes and prosper ratings. The distributions of the interest rates and the original loan
amount will then be presented. We will then going to show the strong positive relationship between the
interest rate/annual percentage rate and loan amount/monthly loan payment.The negative relationship between
interest rates and loan amounts wil then be presented.Then we are going to show the relationship between 
loan outcomes vs interest rates and loan outcomes vs loan amount. After that we are
going to present the relationship between interest rates and prosper ratings. Finally we will present the
interaction between interest rates and loan amounts across loan outcomes and prosper ratings.

## Key Insights for The Presentation

- There is a strong positive relationship between interest rate and annual percentage rate (APR)
- There is a strong positive relationship between original loan amount and monthly loan payments.
- There is a moderate negative relationship between interest rate and the original loan amount.
- There is a linear positive relationship between interest rate and prosper ratings.
- Higher interest rates and lower loan amounts are associated with non-completed loans.
- Higher interest rates and lower loan amounts are associated with Higher-risk ratings.
- Both Higher-risk ratings and non-completed loans are associated with higher interest rates and 
lower loan amounts which may indicate that Prosper ratings are a good estimate for loan outcome.

## Resources

- [Wikipedia article about Prosper](https://en.wikipedia.org/wiki/Prosper_Marketplace)
- [Replacing multiple values in pandas](https://stackoverflow.com/questions/22100130/pandas-replace-multiple-values-one-column)
- [What to consider when creating pie charts](https://academy.datawrapper.de/article/127-what-to-consider-when-creating-a-pie-chart)
- [Correlation betweem two columns in pandas](https://stackoverflow.com/questions/42579908/use-corr-to-get-the-correlation-between-two-columns?noredirect=1&lq=1)
- [Seaborn PairGrid documentation](https://seaborn.pydata.org/generated/seaborn.PairGrid.html)
- [Matplotlib hexbin documentation](https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.pyplot.hexbin.html)
- [seaborn regplot documentation](https://seaborn.pydata.org/generated/seaborn.regplot.html)
