# Prosper Loan Data Exploration
## by Ahmed Mabrouk Fangoh


## Dataset

The dataset involves information on 113937 loans and their borrowers represented using 81 features. The features are mostly of categorical and numerical types. The dataset can be found [here](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554486256021000) and an explainatory dictionary of the variables [here](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554486256024000)


## Summary of Findings

The exploration focused on the relationship between **LoanStatus** and the variables **ProsperScore**, **ListingCategory**, **EmploymentStatus**, **EmploymentStatusDuration**, **IsBorrowerHomeowner**, **OpenRevolvingAccounts**, **DebtToIncomeRatio**, **IncomeRange**, and **LoanOriginalAmount**. This was to conclude if a prediction of the **LoanStatus** is possible from these variables.

Most of the variables showed promising results for correlation with **LoanStatus**. Most notably:
- **ProsperScore** is better at detecting loans likely to be *Completed* but is not very sensitive to *Chargedoff* and *Past Due*
- The **ListingCategories** *Student Use* and *Personal Loan* had the highest percentages of *Completed* loans but also the highest percentages of *Chargedoff* and *Defaulted* loans
- Borrowers with a higher **LoanOriginalAmount** seem to be more likely to be *Past Due* on the loan than have it *Completed*
- There is a tendency for *Full-time* and *Part-time* borrowers with longer **EmploymentStatusDuration** to be *Past Due* on the loan

## Key Insights for Presentation
The presentation illustrates the key findings described in the summary:
- **ProsperScore** may require some tweaking to increase sensitivity to *Chargedoff* and *Past Due*
- The **ListingCategories** *Student Use* and *Personal Loan* seem to be a bit inconsistent with the highest *Completed*, *Chargedoff*, and *Defaulted* percentage of loans
- Due to the correlation noted with **LoanOriginalAmount**, a lower value of this feature is more likely to lead to a completed loan
- The tendency for *Full-time* and *Part-time* borrowers with longer **EmploymentStatusDuration** to be *Past Due* is unusual, and a specific insight could not be concluded from this relationship
