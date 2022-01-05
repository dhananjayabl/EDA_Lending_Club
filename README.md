# Project Name - EDA Lending Club Case Study
> EDA is conducted on Lending Club data to identify driving variables that indicates the loan defaults


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Lending Club  specializes in lending various types of loans to urban customers. LC is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 
Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). The borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters’. 
- Objective of the project is to identifying the risky loan applicant, based on the data available from the loan application and other account and credit history available from other sources like public records. 
- Business Problem: 
    - Accurately identify the risky loan applicants so that appropriate decision can be taken, either to reject the loan application, accept the loan application with higher interest rates or customised repayment schedules
    - Accurately identify the non risky loan applications so that the lending opportunity is not lost
- Analytical Problem:
    - From the given data set identify the driving variables that are indicators of loan default
- Data set used is Lending Club data set has 39717 rows and 111 features

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Continuous values like – ‘loan_amnt’, ‘dti’, ‘revol_bal’ and ‘revol_util’, have clear higher median values for Charge Off and lower median values for Fully Paid
- ‘annual_inc’, has clear higher median value for Fully paid and lower median value for Charge Off
- However, continuous variables on their own has less power to distinguish between risky application vs non-risky application. But when used along with categorical variables like ‘emp_lenght’, ‘verification-status’, they are good indicator of risky application
- This holds same for categorical variables, hence propose the use of categorical variables along with continuous variable to classify risky application
- From our analysis we propose these variables are driving variables that are indicators of risky application;
    - Continuous variables;
        - loan_amt, annual_inc, dti, revol_bal, revol_util
        
    - Categorical variables;
        - emp_length, Verification_status, pub_rec (regrouped), Pub_rec_bankruptcies (regrouped), total_acc (binned), grade, open_acc


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- python - 3.10.1
- pandas - 1.3.5
- numpy - 1.21.5
- matplotlib - 3.5.1
- seaborn - 0.11.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->