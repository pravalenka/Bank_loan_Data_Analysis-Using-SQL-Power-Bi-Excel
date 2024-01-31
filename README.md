# Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel

PROBLEM STATEMENT
-------------------
You can also download from above Problem Statement Document File

DASHBOARD 1: SUMMARY
-----------------------
"In order to monitor and assess our bank's lending activities and performance, we need to create a comprehensive Bank Loan Report. This report aims to provide insights into key loan-related metrics and their changes over time. The report will help us make data-driven decisions, track our loan portfolio's health, and identify trends that can inform our lending strategies.
Key Performance Indicators (KPIs) Requirements:
1.	Total Loan Applications: We need to calculate the total number of loan applications received during a specified period. Additionally, it is essential to monitor the Month-to-Date (MTD) Loan Applications and track changes Month-over-Month (MoM).
2.	Total Funded Amount: Understanding the total amount of funds disbursed as loans is crucial. We also want to keep an eye on the MTD Total Funded Amount and analyse the Month-over-Month (MoM) changes in this metric.
3.	Total Amount Received: Tracking the total amount received from borrowers is essential for assessing the bank's cash flow and loan repayment. We should analyse the Month-to-Date (MTD) Total Amount Received and observe the Month-over-Month (MoM) changes.
4.	Average Interest Rate: Calculating the average interest rate across all loans, MTD, and monitoring the Month-over-Month (MoM) variations in interest rates will provide insights into our lending portfolio's overall cost.
5.	Average Debt-to-Income Ratio (DTI): Evaluating the average DTI for our borrowers helps us gauge their financial health. We need to compute the average DTI for all loans, MTD, and track Month-over-Month (MoM) fluctuations.

Good Loan v Bad Loan KPI’s

In order to evaluate the performance of our lending activities and assess the quality of our loan portfolio, we need to create a comprehensive report that distinguishes between 'Good Loans' and 'Bad Loans' based on specific loan status criteria

Good Loan KPIs:
1.	Good Loan Application Percentage:  We need to calculate the percentage of loan applications classified as 'Good Loans.' This category includes loans with a loan status of 'Fully Paid' and 'Current.'
2.	Good Loan Applications:  Identifying the total number of loan applications falling under the 'Good Loan' category, which consists of loans with a loan status of 'Fully Paid' and 'Current.'
3.	Good Loan Funded Amount:  Determining the total amount of funds disbursed as 'Good Loans.' This includes the principal amounts of loans with a loan status of 'Fully Paid' and 'Current.'
4.	Good Loan Total Received Amount:  Tracking the total amount received from borrowers for 'Good Loans,' which encompasses all payments made on loans with a loan status of 'Fully Paid' and 'Current.'

Bad Loan KPIs:
1.	Bad Loan Application Percentage: Calculating the percentage of loan applications categorized as 'Bad Loans.' This category specifically includes loans with a loan status of 'Charged Off.'
2.	Bad Loan Applications: Identifying the total number of loan applications categorized as 'Bad Loans,' which consists of loans with a loan status of 'Charged Off.'
3.	Bad Loan Funded Amount: Determining the total amount of funds disbursed as 'Bad Loans.' This comprises the principal amounts of loans with a loan status of 'Charged Off.'
4.	Bad Loan Total Received Amount: Tracking the total amount received from borrowers for 'Bad Loans,' which includes all payments made on loans with a loan status of 'Charged Off.'
Loan Status Grid View
In order to gain a comprehensive overview of our lending operations and monitor the performance of loans, we aim to create a grid view report categorized by 'Loan Status.' This report will serve as a valuable tool for analysing and understanding the key indicators associated with different loan statuses. By providing insights into metrics such as 'Total Loan Applications,' 'Total Funded Amount,' 'Total Amount Received,' 'Month-to-Date (MTD) Funded Amount,' 'MTD Amount Received,' 'Average Interest Rate,' and 'Average Debt-to-Income Ratio (DTI),' this grid view will empower us to make data-driven decisions and assess the health of our loan portfolio.

DASHBOARD 2: OVERVIEW
-------------------------
In our Bank Loan Report project, we aim to visually represent critical loan-related metrics and trends using a variety of chart types. These charts will provide a clear and insightful view of our lending operations, facilitating data-driven decision-making and enabling us to gain valuable insights into various loan parameters. Below are the specific chart requirements:

1. Monthly Trends by Issue Date (Line Chart):
Chart Type: Line Chart
Metrics: 'Total Loan Applications,' 'Total Funded Amount,' and 'Total Amount Received'
X-Axis: Month (based on 'Issue Date')
Y-Axis: Metrics' Values
Objective: This line chart will showcase how 'Total Loan Applications,' 'Total Funded Amount,' and 'Total Amount Received' vary over time, allowing us to identify seasonality and long-term trends in lending activities.

2. Regional Analysis by State (Filled Map):
Chart Type: Filled Map
Metrics: 'Total Loan Applications,' 'Total Funded Amount,' and 'Total Amount Received'
Geographic Regions: States
Objective: This filled map will visually represent lending metrics categorized by state, enabling us to identify regions with significant lending activity and assess regional disparities.

3. Loan Term Analysis (Donut Chart):
Chart Type: Donut Chart
Metrics: 'Total Loan Applications,' 'Total Funded Amount,' and 'Total Amount Received'
Segments: Loan Terms (e.g., 36 months, 60 months)
Objective: This donut chart will depict loan statistics based on different loan terms, allowing us to understand the distribution of loans across various term lengths.

4. Employee Length Analysis (Bar Chart):
Chart Type: Bar Chart
Metrics: 'Total Loan Applications,' 'Total Funded Amount,' and 'Total Amount Received'
X-Axis: Employee Length Categories (e.g., 1 year, 5 years, 10+ years)
Y-Axis: Metrics' Values
Objective: This bar chart will illustrate how lending metrics are distributed among borrowers with different employment lengths, helping us assess the impact of employment history on loan applications.

5. Loan Purpose Breakdown (Bar Chart):
Chart Type: Bar Chart
Metrics: 'Total Loan Applications,' 'Total Funded Amount,' and 'Total Amount Received'
X-Axis: Loan Purpose Categories (e.g., debt consolidation, credit card refinancing)
Y-Axis: Metrics' Values
Objective: This bar chart will provide a visual breakdown of loan metrics based on the stated purposes of loans, aiding in the understanding of the primary reasons borrowers seek financing.

6. Home Ownership Analysis (Tree Map):
Chart Type: Tree Map
Metrics: 'Total Loan Applications,' 'Total Funded Amount,' and 'Total Amount Received'
Hierarchy: Home Ownership Categories (e.g., own, rent, mortgage)
Objective: This tree map will display loan metrics categorized by different home ownership statuses, allowing for a hierarchical view of how home ownership impacts loan applications and disbursements.
These diverse chart types will enhance our ability to visualize and communicate loan-related insights effectively, supporting data-driven decisions and strategic planning within our lending operations."

DASHBOARD 3: DETAILS
----------------------
In our Bank Loan Report project, we recognize the need for a comprehensive 'Details Dashboard' that provides a consolidated view of all the essential information within our loan data. This Details Dashboard aims to offer a holistic snapshot of key loan-related metrics and data points, enabling users to access critical information efficiently.
Objective:
The primary objective of the Details Dashboard is to provide a comprehensive and user-friendly interface for accessing vital loan data. It will serve as a one-stop solution for users seeking detailed insights into our loan portfolio, borrower profiles, and loan performance.

####################################################################################################

 USING SQL 
 ---------
BANK LOAN REPORT QUERY DOCUMENT
A.BANK LOAN REPORT | SUMMARY

KPI’s:

1. Total Loan Applications

SELECT COUNT(id) AS Total_Applications FROM bank_loan_data

![Total_application](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/d9afa04c-8684-458b-87cd-a76bac694f1d)

2. MTD Loan Applications

SELECT COUNT(id) AS Total_Applications FROM bank_loan_data
WHERE MONTH(issue_date) = 12

![MTD Loan Applications](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/391b7160-1074-4425-b35e-f8c8df5ed7f8)

3. PMTD Loan Applications

SELECT COUNT(id) AS Total_Applications FROM bank_loan_data
WHERE MONTH(issue_date) = 11

 ![PMTD Loan Applications](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/f1618879-dc21-4f96-8d2b-5b2fcaa2964d)

4. Total Funded Amount

SELECT SUM(loan_amount) AS Total_Funded_Amount FROM bank_loan_data

![Total Funded Amount](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/51745ac3-8236-400c-8186-80de9fd213ce)

5. MTD Total Funded Amount
   
SELECT SUM(loan_amount) AS Total_Funded_Amount FROM bank_loan_data
WHERE MONTH(issue_date) = 12

![MTD Total Funded Amount](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/f7bf3838-1d01-4a82-b792-8e60491ee4b0)

6. PMTD Total Funded Amount
   
SELECT SUM(loan_amount) AS Total_Funded_Amount FROM bank_loan_data
WHERE MONTH(issue_date) = 11

 ![PMTD Total Funded Amount](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/befccb18-b738-440d-b2c6-5e9247fead3c)

7. Total Amount Received
   
SELECT SUM(total_payment) AS Total_Amount_Collected FROM bank_loan_data

![Total Amount Received](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/302829e1-b276-42b3-a084-1036f95ea21e)

8. MTD Total Amount Received
   
SELECT SUM(total_payment) AS Total_Amount_Collected FROM bank_loan_data
WHERE MONTH(issue_date) = 12

![MTD Total Amount Received](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/a0baed9c-5066-427a-9e2d-a2327089cf21)

9. PMTD Total Amount Received
    
SELECT SUM(total_payment) AS Total_Amount_Collected FROM bank_loan_data
WHERE MONTH(issue_date) = 11

![PMTD Total Amount Received](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/7487fb91-af25-4655-95a2-87d1dde30181)

10. Average Interest Rate
SELECT AVG(int_rate)*100 AS Avg_Int_Rate FROM bank_loan_data


![Average Interest Rate](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/109ca276-e8c6-447f-a1a7-4e16e40e7c5d)

11. MTD Average Interest
    
SELECT AVG(int_rate)*100 AS MTD_Avg_Int_Rate FROM bank_loan_data
WHERE MONTH(issue_date) = 12

![MTD Average Interest](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/036f6c1e-be2c-4f9c-b8c1-d105978ab792)

12. PMTD Average Interest
    
SELECT AVG(int_rate)*100 AS PMTD_Avg_Int_Rate FROM bank_loan_data
WHERE MONTH(issue_date) = 11

![PMTD Average Interest](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/8e87e143-8902-409b-a020-b05c3a6fbfa0)

13. Avg DTI
    
SELECT AVG(dti)*100 AS Avg_DTI FROM bank_loan_data

![Avg DTI](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/82750358-a37d-4c83-bd7c-516ac9d70fb7)

14. MTD Avg DTI
    
SELECT AVG(dti)*100 AS MTD_Avg_DTI FROM bank_loan_data
WHERE MONTH(issue_date) = 12

![MTD Avg DTI](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/255ec0b9-a6d4-47b9-8542-cf01af5b644a)

15. PMTD Avg DTI
    
SELECT AVG(dti)*100 AS PMTD_Avg_DTI FROM bank_loan_data
WHERE MONTH(issue_date) = 11

 ![PMTD Avg DTI](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/a06ed084-3616-41e6-a59b-df6ca8056f1c)

16. GOOD LOAN ISSUED
  
1. Good Loan Percentage
   
SELECT
    (COUNT(CASE WHEN loan_status = 'Fully Paid' OR loan_status = 'Current' THEN id END) * 100.0) / 
	COUNT(id) AS Good_Loan_Percentage
FROM bank_loan_data

![Good Loan Percentage](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/6bd2762b-01bc-4e08-b194-80ee2cacd8a6)

2. Good Loan Applications
   
SELECT COUNT(id) AS Good_Loan_Applications FROM bank_loan_data
WHERE loan_status = 'Fully Paid' OR loan_status = 'Current'

![Good Loan Applications](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/d987e6a4-6dda-42c7-a873-f0a07fd877cc)

3. Good Loan Funded Amount
   
SELECT SUM(loan_amount) AS Good_Loan_Funded_amount FROM bank_loan_data
WHERE loan_status = 'Fully Paid' OR loan_status = 'Current'

![Good Loan Funded Amount](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/dfa11b49-e5dc-43ec-af67-91c5af482b6b)

4. Good Loan Amount Received
   
SELECT SUM(total_payment) AS Good_Loan_amount_received FROM bank_loan_data
WHERE loan_status = 'Fully Paid' OR loan_status = 'Current'

![Good Loan Amount Received](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/87a847f9-7400-4c62-9595-e9cbf741731a)

17. BAD LOAN ISSUED

1. Bad Loan Percentage

SELECT
    (COUNT(CASE WHEN loan_status = 'Charged Off' THEN id END) * 100.0) / 
	COUNT(id) AS Bad_Loan_Percentage
FROM bank_loan_data

![Bad Loan Percentage](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/1fcf847b-9498-476e-9430-d6ebeec7552f)

2. Bad Loan Applications
   
SELECT COUNT(id) AS Bad_Loan_Applications FROM bank_loan_data
WHERE loan_status = 'Charged Off'

![Bad Loan Applications](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/3579cfa6-664e-4202-857d-28b27d109f2b)

3. Bad Loan Funded Amount
   
SELECT SUM(loan_amount) AS Bad_Loan_Funded_amount FROM bank_loan_data
WHERE loan_status = 'Charged Off'

![Bad Loan Funded Amount](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/6a204f84-bc7d-4f7d-a0f8-178f8c4ded8a)

4. Bad Loan Amount Received
   
SELECT SUM(total_payment) AS Bad_Loan_amount_received FROM bank_loan_data
WHERE loan_status = 'Charged Off'

![Bad Loan Amount Received](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/66e152bd-1498-432e-94a0-e7f04088a7eb)

18. LOAN STATUS
    
	SELECT
        loan_status,
        COUNT(id) AS LoanCount,
        SUM(total_payment) AS Total_Amount_Received,
        SUM(loan_amount) AS Total_Funded_Amount,
        AVG(int_rate * 100) AS Interest_Rate,
        AVG(dti * 100) AS DTI
    FROM
        bank_loan_data
    GROUP BY
        loan_status
 
SELECT 
	loan_status, 
	SUM(total_payment) AS MTD_Total_Amount_Received, 
	SUM(loan_amount) AS MTD_Total_Funded_Amount 
FROM bank_loan_data
WHERE MONTH(issue_date) = 12 
GROUP BY loan_status
 
![LOAN STATUS](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/277a0e44-8421-4d75-a079-c690bbf9db23)
![LOAN STATUS1](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/79f9b95c-c405-40ca-adad-8dba5ecc4cfc)


B. BANK LOAN REPORT | OVERVIEW

1. MONTH
   
SELECT 
	MONTH(issue_date) AS Month_Munber, 
	DATENAME(MONTH, issue_date) AS Month_name, 
	COUNT(id) AS Total_Loan_Applications,
	SUM(loan_amount) AS Total_Funded_Amount,
	SUM(total_payment) AS Total_Amount_Received
FROM bank_loan_data
GROUP BY MONTH(issue_date), DATENAME(MONTH, issue_date)
ORDER BY MONTH(issue_date)

![Month](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/70037ce9-fd1a-4b7c-bacb-1b02de6482dc)

2. STATE
   
SELECT 
	address_state AS State, 
	COUNT(id) AS Total_Loan_Applications,
	SUM(loan_amount) AS Total_Funded_Amount,
	SUM(total_payment) AS Total_Amount_Received
FROM bank_loan_data
GROUP BY address_state
ORDER BY address_state

![STATE](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/6bbca16d-b787-453c-b826-dd46ba2c8e82)

3. TERM
   
SELECT 
	term AS Term, 
	COUNT(id) AS Total_Loan_Applications,
	SUM(loan_amount) AS Total_Funded_Amount,
	SUM(total_payment) AS Total_Amount_Received
FROM bank_loan_data
GROUP BY term
ORDER BY term

![TERM](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/7b6b79a2-38ad-418b-a092-1707e6617d7d)

4. EMPLOYEE LENGTH
   
SELECT 
	emp_length AS Employee_Length, 
	COUNT(id) AS Total_Loan_Applications,
	SUM(loan_amount) AS Total_Funded_Amount,
	SUM(total_payment) AS Total_Amount_Received
FROM bank_loan_data
GROUP BY emp_length
ORDER BY emp_length

![EMPLOYEE LENGTH](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/25fb3fa5-3bfd-4b5f-91b5-aa5058f0e5a7)

5. PURPOSE
   
SELECT 
	purpose AS PURPOSE, 
	COUNT(id) AS Total_Loan_Applications,
	SUM(loan_amount) AS Total_Funded_Amount,
	SUM(total_payment) AS Total_Amount_Received
FROM bank_loan_data
GROUP BY purpose
ORDER BY purpose

![PURPOSE](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/0496271d-bd69-453b-994e-90224e1942af)

6. HOME OWNERSHIP
   
SELECT 
	home_ownership AS Home_Ownership, 
	COUNT(id) AS Total_Loan_Applications,
	SUM(loan_amount) AS Total_Funded_Amount,
	SUM(total_payment) AS Total_Amount_Received
FROM bank_loan_data
GROUP BY home_ownership
ORDER BY home_ownership

![HOME OWNERSHIP](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/bd8eb4ff-40d5-494e-a419-f8a2442a1627)

--Note: I have applied multiple Filters on all the dashboards. You can check the results for the filters as well by modifying the query and comparing the results.
For e.g-

7. See the results when we hit the Grade A in the filters for dashboards.

SELECT 
	purpose AS PURPOSE, 
	COUNT(id) AS Total_Loan_Applications,
	SUM(loan_amount) AS Total_Funded_Amount,
	SUM(total_payment) AS Total_Amount_Received
FROM bank_loan_data
WHERE grade = 'A'
GROUP BY purpose
ORDER BY purpose

![See the results when we hit the Grade A in the filters for dashboards](https://github.com/pravalenka/Bank_loan_Data_Analysis-Using-SQL-Power-Bi-Excel/assets/120097217/81f8bef3-51e7-4ed8-a8d9-743ae4ff332a)


