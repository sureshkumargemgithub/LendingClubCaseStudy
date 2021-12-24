# LendingClubCaseStudy
> A study for seeing the pattern which customers most probably default the loans so that more cautious decisions can be made while approving the loans

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- Problem statement for the lending club financial institution is to identify the patterns or big factors which could probably lead to default the loan by customers
- By using EDA, if we can identify those hidden patterns or behaviour will give the flexibility for the institution to stop such loans or take other precautions
- Borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 
- This will reduce major credit loss for the bank because it will put very big risk to the bank or any institution if the loan has to be charged-off.
- A dataset is getting used here to find out the factors. Dataset contains the customers personal identification inforation, finanical information, loan details, payment details and so on...

## Technologies Used
- Python library - version 3
- Jupyter Notebook - Anaconda 3
- Git and GitHub for creating the repo to share it publicly

## Assumptions
- This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface.

## Observations
- The loan amount varies from 0 to 35,000 having mean of 10,000
- Most of the loans have grade of A and B and also Grade B is the mostly issued loan.
- Funded amount is left skewed. Most of the loan amount given is 10,000 and next high frequent loan is 5000 and around 5K
- Majority of loan applicants have income less than 1 lakh.
- Note: We are not showing here but observed that if we remove outliers on income with formula df[~((df < (Q1 - 1.5 * IQR)) |(df > (Q3 + 1.5 * IQR)))] then half of population falls under 40 to 80 thousand income level
- Most of the loans are issued either to people with more than 10 years of experience or early in their job (upto 3 years of experience)

## Conclusions
- Its very clear that higher interest rate leading to many charge offs
- About 50% of defaults are under debt consolidation, it is as a result of majority of loans being sanctioned for the purpose of debt consolidation. On the other hand, only a small portion of loans are sanctioned for small businesses, more than 20% of these are charged off as oppose to about 15% with debt consolidation. Therefore, loans for small businesses should be approved with caution.
- If we observe the number of loans, we found that majority of loans are given for a term of 36 months. After, looking at loan_status , we find that higher proportion of 60 month loan are charged off compared to 36 month. It seems 60 month loans are more risky and therefore are rightfully issued sparingly.
- Mortgage and Rent people are more likely to pay based on the Fully Paid and Charged Off percentages. But Own house customers are less likely to pay. But does not seem very strong factor.
- Looks very strong indicator that 0 times bankrupted customers very likely to pay, 1 time is okay but risky and 2 times is very much unlikely to pay
- "Very high" loan_inc_ratio_range or dti range customers are less likey to pay as it is clearly visible difference. Charge Off became darker and Fully Paid became lighter at this range


## Acknowledgements
- This project is our first upGrad assignment to predict less likely paying customers so that approving loans can be easier.


## Contact
Created by [@sureshkumargemgithub] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
