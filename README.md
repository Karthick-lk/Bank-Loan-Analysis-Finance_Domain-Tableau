# Bells Bank Loan Analysis

## Problem Statement
Bells Bank, is a fictional bank in the USA and it is one of the top prioritized bank by people for borrowing loans. The stakeholders of the bank wants to gain insights about the health of banks's loan portfolio and asks the data anlytics team to analyze the historical data to find trends and patterns. These trends and pattern will help in data-driven decision making for the stakeholders and enhance the bank's loan portfolio.

## Requirements from the Stakeholders
1. **Key Performance Indicators**
    - Total Loan Applications (Month to Date, Month over Month)
    - Total Funded Amount (Month to Date, Month over Month)
    - Total Amount Received (Month to Date, Month over Month)
    - Average Interest Rate (Month to Date, Month over Month)
    - Average Debt-to-Income Ratio (Month to Date, Month over Month)
      
2. **Good/Bad Loan KPI's**
    - Good/Bad Loan Application Percentage
    - Good/Bad Loan Total Applications
    - Good/Bad Loan Total Funded Amount
    - good/Bad Loan Total Received Amount

3. **Loan-Related Metrics and Trends**
    - Monthly Trends by Issue Date
    - Regional Trends by State
    - Loan Term Analysis
    - Employee Length Analysis
    - Loan Purpose Breakdown
    - Home Ownership Analysis

## Dataset
**financial_loan.csv** : The dataset contains columns like id, address_state, application_type emp_length, emp_title, grade, home_ownership, home_ownership, issus_date, last_credit_pull_date, last_payment_date, loan_status, next_payment_date, member_id, purpose, sub_grade, term, verification_status, annual_income, dti, installment, int_rate, loan_amount, total_acc, total_payment. 

## Implementing SQL for Stakeholders requirements
1. **Total Loan Applications (Month to Date, Month over Month)**                               
    - select count(*) as Total_Loan_Applications from financial_loan;                                 

    - select count(*) as MTD_Total_Loan_Applications from financial_loan                                              
      where MONTH(issue_date) = 12 and YEAR(issue_date)=2021;                                    

    - select count(*) as PMTD_Total_Loan_Applications from financial_loan                                       
      where MONTH(issue_date) = 11 and YEAR(issue_date)=2021;
2. **Total Funded Amount (Month to Date, Month over Month)**
    - select SUM(loan_amount) as Total_Funded_Amount from financial_loan;

    - select sum(loan_amount) as MTD_Total_Funded_Amount from financial_loan
      where MONTH(issue_date) = 12 and YEAR(issue_date)=2021;

    - select sum(loan_amount) as PMTD_Total_Funded_Amount from financial_loan
      where MONTH(issue_date) = 11 and YEAR(issue_date)=2021;
                                               


## Dashboard Live here

## Dashboard Created





















