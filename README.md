# Prosper-Loan
Analysis of prosper loan data.  

## Dataset

Prosper was founded in 2005 as a peer-to-peer online lending marketplace in the United States. Borrowers apply online for a fixed-rate, fixed-term loan and investors (individual or institutional) can fund anywhere from $\$$2,000 to $\$$40,000 per loan request to earn returns. These investors can consider borrowers’ credit scores, ratings, history and the category of the loan.  

The dataset contains 113,937 loans on Proper's marketplace with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. It can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv), with feature documentation available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0). 

Common issues such as nulls and duplicates were sorted, categorical variables ordered and a tidiness issue where variables were scattered accross columns was fixed. After cleaning, the resulting dataset had 26 features of about 112238 loans from 2005 to 2014.


## Summary of Findings
Exploration of the dataset reveals that; 

There is a strong relationship between borrowers annual percentage rate and estimated loss. An increase in the rate at which prosper profits(interest rate) from a loan means an increase in the amount that could be lost from that loan. These features are negatively associated with credit rating in that higher APR and estimated loss are assigned to loans taken by borrowers with low credit rating. There was also a negative association between estimated loss and (categorical)-borrowers' financial features in the dataset as borrowers with higher prosper score, income range or credit rating had lower loss estimates. Investors seemed to take this into cognizance as their numbers decreased with inreasing loss estimates on loans.

Although Prosper infrequently had occasions where they made losses, with just over 15k loans resulting in losses from over 110k;  they made actual losses on a large proportion of loans from inception till 2009 which was usually via defaults from high risk borrowers. It is noticed that higher amounts lost per loan are associated with loans assigned low loss estimates.

Outside of the main variables of interest;

* Delinquents reduced with higher credit ratings.
* Loan term had a postive correlation with amount borrowed(large amount borrowed indicated longer loan terms).
* Debt Consolidation was the main reason why people took loans from prosper, followed by the desire to fund home improvement projects.
* The proportion of borrowers who were homeowners just slightly edges those who are not, with approximately 51% and 49% respectively. 
* The largest percentage of borrowers were from California. The rest, Texas, Florida, New York and Illinois were also ranked in top 5 most populous states in the USA.
* Just less than 8% of borrowers could not verify their income.
* There is a clear growth in the amount of loans taken on prosper until 2014.


## Key Insights for Presentation

For the presentation, focus is placed on the influence of credit rating on borrower APR, estimated loss and net loss. Also, the loan patterns of users(verified and unverified) in a credit rating would be presented.
