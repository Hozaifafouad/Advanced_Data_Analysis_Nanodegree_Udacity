# Visualization-analysis of Loan dataset
This analysis is a part of Advanced data-analysis nano-degree provided by Udacity and sponsored by FWD

## Dataset
The [`dataset`](https://github.com/HamzaFouad/Advanced_Data_Analysis_Udacity/blob/master/3_visualization_analysis/prosperLoanData.csv) we will be using is a loan dataset, it contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. -   This [`data dictionary`](https://github.com/HamzaFouad/Advanced_Data_Analysis_Udacity/blob/master/3_visualization_analysis/schema_ProsperLoanData.csv) explains the variables in the dataset.
We will be focusing on just a few variables and focus on answering these questions:
* What factors affect a loan’s outcome status?
* What affects the borrower’s APR or interest rate?

## Summary of Findings

* Interestingly, most of the borrowers in this dataset seems to be put in D-category.
* LoanOriginalAmount, StatedMonthlyIncome and Investors distributions are highly right-skewed.
* There is a negative correlation between Investors and BorrowerAPR.
* The monthy loan payment increases as the Original loan increases.
* People with the lower incomeRange tend to have higher average APR, it is strange though.
	* mabye due to their payment-delay?
	* or maybe due to they have less investors?
	* or mabye due to the fact that these people tend to NEED loans more than the other (e.g. for houses or Autos ..etc.).
We will see the relation between IncomeRange and the others to see why lower income range have higher APR.
* People with lower income range tend to have fewer investors.
* Invistors increase is indication of a good ProsperRating.
* The HIGHEST APR tends to go for Household Expenses followed by Medical expenses.
* APR decreases as the LoanOriginalAmount increases.
* Borrowers with their own houses tend to complete the loan more than the others.
* Number of Chargedoff borrowers tend to follow the ProsperRating scale, as risk increases charing increases which is pretty obvious :D
* Ratio between people with higher IncomeRange who own houses to who don't is higher than the people with lower IncomeRange.
* As MonthlyIncome increases, the borrower gain a good prosperrating and eventually he completes the loan.
* Here is interesting results, if the monthly loan payment increased over a certain point, EVEN IF the borrower is considered in a AA-ProsperRating-category, debt is unlikely to be collected.
<hr>

### As a summary to the above questions
* Employed borrowers, obviously, have higher monthly income, and as the monthly income increases the prosper rating increases and eventually they more likely to complete their loan.  
* HouseOwner-borrowers are likely to complete their loan compared to the borrowers who don't have houses.  
* Investors increase is an indication of a good prosper rating, and eventually the borrower is likely to complete the loan.  
      
* APR is mainly affected by the original amount of loan, and the Listing category for the loan.  
    interestingly, APR increases as the original amount of loan increases. and the highest APR-listing-category is Household expenses followed by medical expenses.  
* APR is also affected by the borrower income-range. it increases as the income-range decreases.