# Prosper Loan Data Exploration
## by Garainesu Hove

## Dataset

The data consists of information regarding 115,000 loan, including 81 variables
The dataset can be found is provided by Udacity.  

## Summary of Findings

I've found that Borrower APR and Credit Score Range Lower has negative moderate
correlation. Borrower APR has moderate negative correlation with
LoanOriginalAmount too. CreditScoreRangeLower and LoanOriginalAmount are
moderately positively correlated.

Business Category is likely to have higher Credit Score. Loan status of
Borrowers who have higher credit score are more likely to be completed. Also
loans with lower BorrowerAPR are likely to be completed too which is also
expected. CreditScoreRangeLower is generally lower for borrowers
who has income verifiable.

The higher the income range the higher credit score. Borrowers with low income
range likely to have higher Borrower APR. 

Category labeled as "Student Use" are more likely to have lower stated monthly
income which may be related with lower credit scores.

Borrowers who has income not verifiable are more likely to apply for Business
Category. The borrowers with income not verifiable has a lot higher proportion
of Business Category than income verifiable.

Most of borrowers with income not verifiable are self employed.

Highest defaulted and chargedoff rates are in lower income ranges which is
expected.

## Key Insights for Presentation

For the presentation, I started introducing three variables of interest:
(Loan Status, Borrower APR and Credit Score Range Lower) then followed by
two categorical variables, Income Range and Borrower State. Then I scatterplot
two moderately correlated pairs with one of them is variable of interest.

Afterwards, I include categorical variables Loan Status, Is Borrower Home Owner
Is Income Verifiable and Income Range into numerical variables of interest
using heatmap (Credit Score Range Lower and Borrower APR)

## List of Resources

I learned type of loan status from these resources:
https://www.investopedia.com/terms/c/cancellation-of-debt.asp
https://www.valuepenguin.com/loans/what-does-it-mean-to-default-on-a-loan
https://www.investopedia.com/terms/c/chargeoff.asp

I used this stackoverflow source to convert value_counts to a dataframe:
https://stackoverflow.com/questions/47136436/python-pandas-convert-value-counts-output-to-dataframe

remove y axis: get help from:
https://stackoverflow.com/questions/2176424/hiding-axis-text-in-matplotlib-plots

remove frames, get help from:
https://stackoverflow.com/questions/14908576/how-to-remove-frame-from-matplotlib-pyplot-figure-vs-matplotlib-figure-frame

I've found from here a way to show proportions in y axis for bivariate
exploration:
https://github.com/mwaskom/seaborn/issues/1027
