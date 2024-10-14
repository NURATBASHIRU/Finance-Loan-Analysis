## Title: Finance Loan Analysis – Overview, Customers Segmentation and Risk Analysis.

#### Objective 
Just like every other institution, it is important to perform periodical analysis on business performance in order for this companies to make data-driven decisions. Therefore, this analysis was performed for a finance loan institution in the United States. This company wants to understand the level of loan default it is experiencing and the factors that contributes to it default rate. As a result, a data analysis procedure was performed in order to answer a few key questions;
-	What is the effect of interest rate on loan acquired by borrowers?
-	Which loan purpose has the highest loan approval and default rate?
-	How does the customer verification status affect the default rate?
-	How does the loan term affect the default rate?
-	Who are our borrowers and how do they fit into a common spectrum?
-	What is the loan approval and default rate for each state?
In order to answer these questions, I created a three-way dashboard, projecting the Overview, Customers Segmentation and Risk Analysis.

#### Methodology;
-	Tool: Microsoft Excel
-	Technique: Using the member’s LTV (Loan To Value) Ratio and DTI (Debt To Income) Ratio, I was able to group these customers based on similar earning / debt category.
-	Process: I performed an intensive data transformation procedure on the dataset and the procedure required me to create a few new columns. As a result, the dataset increased from 26 columns and 38,590 rows to 30 columns and 38,575 rows.

#### Data Transformation Process
Transforming this dataset would have been a little more difficult if a “data dictionary” was not created by TDI. However, the following are the data transformation process the dataset went through;
1.	Data Cleaning: I performed an overall data cleaning procedure using; trim, proper and text functions to remove excess space and format the data appropriately.
2.	Blanks: I used the Find and Replaced feature of Excel to replace empty cells in “job role” column with “others” – so that all members can be evenly categorized. I also did the same with the “total payment” column. I replaced empty cells in “total payment” column with 0
3.	Data Manipulation: I used VLOOKUP function to convert the “Address State” column from Alpha 2 area code to actual state name. I used the IF statement to group the interest rate into 3 categories – “low interest rate”, “mid interest rate” and “high interest rate”. I converted “Home Ownership” column from abbreviation to words; Home ownership status of members was in “R, MO, O, NONE format” (R-RENT, MO- MORTGAGE, O-OWN). I applied the same process for the “Verification Status” column as it was in; V-Verified, NOT V- Not Verified, SV- Source Verified format
4.	Metrics Generation: I created a new column – LTV - derived LTV (Loan to Value) by using “Annual income” as collateral. So, LTV = Loam amount/Annual Income X 100. I also created a “loan Deficit” Column by using; loan amount - Total payment

#### Insights
1.	The finance company has a total loan approval rate of $473 million all through the year; with a $435.7 million retrieved and a default of -$37.3 million - losing about 10% of its principal. 
2.	The finance company has been approving loans for customers whose biodata and collateral value are not verified. This could be directly associated with high default rate; since customer details are not verified, it makes it easy for the borrowers to fail to perform their responsibility.
3.	The loan loan term is another factor directly responsible for the high default rate as majority of these borrowers opt for the shorter loan term and by implication, are unable to meet up with time.
4.	Borrowers who have long term work experience have the highest default rate. This could be linked to debt accumulation over the years as ‘debt consolidation’ has the highest loan approval and default rate.
5.	Interest rate has the same impact on loan performance - the higher the interest rate, the more members borrow
6.	Members who own houses on mortgage have the highest loan approval rate followed by members who live in rented houses. While members who own their homes get a really low percentage of loan approval. This draws us back to customer verification being a key factor to default rate as customers who don’t own a house barely have any property to lose.
 members who do not own a house barely get loan approval - for obvious reasons.
7.	California, New York and Texas are the highest loan approval rate and consequently, the highest default rate. 

#### Recommendations 
1.	The finance company should review it loan policy generally to reduce loan defaults 
2.	The company should ensure proper assessment of collateral value, debt to income ratio and customer verification before approving loan application.
3.	The company should increase it loan approval rate for home owners - as long as the borrower’s property meets the collateral policy. Since customers who own house properties have a lot more to lose.
4.	The company should develop a more strategic loan term that will be convenient for both parties.
