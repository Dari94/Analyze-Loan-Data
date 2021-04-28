# Analyze-Loan-Data

## Dataset
Original dataset contains 113937 loans with 81 variables on each loan, including loan amount, Borrower APR, current loan status, borrower income,Prosper Rating, BorrowerState, Occupation and many others.Each entry gives us idea about the borrower and it's background and the details of the loan associated with them.

## Summary of Findings
During exploration I wanted to figure out what features are best for predicting the borrower's Annual Percentage Rate (APR) for the loan and how employment status, Ocupation and Prosper Rating associates with various metrics in the dataset.

I expect that the Loan Original Amount will have a negative effect on the Borrower APR(Anual Percentage Rate) because with the increase of loan amount I expect APR to get lower. I suspect that the employment status, occupation and monthly income will have an effect on the Borrower APR. These characteristics will aslo affect Loan Amount and Prosper Rating.

BorrowerAPR distribution seems fairly normal with an exception of very high peak around ~0.35. Only very few loans have APR greater than 0.43.

The distribution of Stated Monthly Income is right skewed. The peak is around 6K. More of the monthly incomes are less than 30K except some outliers around 50K which should be removed

The distribution of original loan amount have very large spikes in frequency 5K, 10K, 15K, 20K, 25K. It means that most of the loans are multiples of 5k.

From the correlation between Borrower APR and Occupation or Employment Status categorical variables I found out that Occupation and Employment Status are not affected significantly the Borrower ARR.

From distribution of loan listed by year and month I found out that there is an upper trend in loans listing yeach passing year. The year with the maximum loans is 2013 year. January is the month with the highest number of loan swhereas April is the month with the least number of loans listed.


The correlation coefficient of borrower APR and loan original amount is -0.426( noticed from the heatmap), the scatter plot also shows that these two variables are negatively correlated,following that the more the loan amount is, the lower the APR. The negative corelation between 'ProsperScore' and 'BorrowerAPR' and the positive correlation between 'Loan Original Amount' and 'Monthly Loan Payment' are also shown in scaterplot.

The borrower APR decreases with the better rating. Borrowers with the best Prosper ratings have the lowest APR. It means that the Prosper rating has a strong effect on borrower APR. Borrowers with better rating also have larger monthly income and loan amount. Employed, self-employed and full time borrowers have more monthly income and loan amount than part-time, retired and not employed borrowers.

The loan amount increases with better rating. The borrower APR decreases with better rating. Interestingly, the relationship between borrower APR and loan amount turns from negative to slightly positive when the Prosper ratings are increased from HR to A or better. This may because people with A or AA ratings tend to borrow more money, increasting APR could prevent them borrow even more and maximize the profit. But people with lower ratings tend to borrow less money.

Interestingly, the borrower APR decrease with the increase of borrow term for people with HR-C raings. But for people with B-AA ratings, the APR increase with the increase of borrow term.
There is an interaction between term and rating for Loan Original Amount. With better Prosper rating, the loan amount of all three terms increases, the increase amplitude of loan amount between terms also becomes larger.
## Key Insights for Presentation
BorrowerAPR distribution seems fairly normal with an exception of very high peak around ~0.35. There are small peaks centered at 0.1 and 0.2. Only very few loans have APR greater than 0.4

There is an upper trend in loans listing yeach passing year. The year with the maximum loans is 2013 year. January is the month with the highest number of loan swhereas April is the month with the least number of loans listed.


Borrower APR and Original Loan Amount are negatively correlated,following that the more the loan amount is, the lower the APR.

The borrower APR decreases with the increasingly better rating. Borrowers with the best Prosper ratings have the lowest APR. It means that the Prosper rating has a strong effect on borrower APR.

Prosper Score and Borrower APR are Negatively correlated.

The borrower APR decreases with better rating and the loan amount increases with better rating. The relationship between borrower APR and loan amount turns from negative to slightly positive when the Prosper ratings are increased from HR to A or better.

Interesting finding is that for people with prosper ratings B-AA, the APR increase with the increase of borrow term and for people with prosper ratings HR-C the APR decrease with the increase of borrow term.

The borrower APR changes with the occupation. Junior Students having highest Borrower APR and judges having lowest.Most of the people who get loans are from either professional or other occupation. Loans for 36 months are preffered by most of the people and the 12 month duration for repaymen is the least preffered

