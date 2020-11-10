# Credit-Card-Approval-Prediction
- Credit score cards are a common risk control method in the financial industry. It uses personal information and data submitted by credit card applicants to predict the probability of future defaults and credit card borrowings. The bank is able to decide whether to issue a credit card to the applicant. Credit scores can objectively quantify the magnitude of risk. 
- In this project we are trying to build Machine Learning model to predict if an applicant is 'good' or 'bad' client i.e if applicat is 'Risky' or 'Not'. 
- Here 'Risk' == 'Yes' === 1 &amp; 'Risk' == 'No' === 0

# Content & Explaination
- - Generally speaking, credit score cards are based on historical data. Once encountering large economic fluctuations. Past models may lose their original predictive power. Logistic model is a common method for credit scoring. Because Logistic is suitable for binary classification tasks and can calculate the coefficients of each feature. In order to facilitate understanding and operation, the score card will multiply the logistic regression coefficient by a certain value (such as 100) and round it.
- At present, with the development of machine learning algorithms. More predictive methods such as Boosting, Random Forest, and Support Vector Machines have been introduced into credit card scoring. However, these methods often do not have good transparency. It may be difficult to provide customers and regulators with a reason for rejection or acceptance.

# Dataset Description
- There're two tables could be merged by ID:

1. Table 1
    1. ID ----------------------- 	Client number 	
    2. CODE_GENDER --------------	Gender 	
    3. FLAG_OWN_CAR -------------	Is there a car 	
    4. FLAG_OWN_REALTY ----------	Is there a property 	
    5. CNT_CHILDREN -------------	Number of children 	
    6. AMT_INCOME_TOTAL ---------	Annual income 	
    7. NAME_INCOME_TYPE ---------	Income category 	
    8. NAME_EDUCATION_TYPE ------ 	Education level 	
    9. NAME_FAMILY_STATUS -------	Marital status 	
    10. NAME_HOUSING_TYPE -------	Way of living 	
    11. DAYS_BIRTH --------------	Birthday ------------------- Count backwards from current day (0), -1 means yesterday
    12. DAYS_EMPLOYED -----------	Start date of employment --- Count backwards from current day(0). If positive, it means the person currently unemployed.
    13. FLAG_MOBIL --------------	Is there a mobile phone 	
    14. FLAG_WORK_PHONE ---------	Is there a work phone 	
    15. FLAG_PHONE --------------	Is there a phone 	
    16. FLAG_EMAIL --------------	Is there an email 	
    17. OCCUPATION_TYPE ---------	Occupation 	
    18. CNT_FAM_MEMBERS ---------	Family size

2. Table 2

    1. ID ---------------	Client number 	
    2. MONTHS_BALANCE --- 	Record month ---- The month of the extracted data is the starting point, backwards, 0 is the current month, -1 is the previous month, and so on
    3. STATUS -----------	Status ---------- 0: 1-29 days past due 1: 30-59 days past due 2: 60-89 days overdue 3: 90-119 days overdue 4: 120-149 days overdue 5: Overdue or bad debts, write-offs for more than 150 days C: paid off that month X: No loan for the month
    
 # Approach for Problem Solving
1. Understanding the Problem
2. Downloading the Dataset
3. Importing necessary Dependencies
4. Exploratory Data Analysis
5. Data Pre-Processing
6. Feature Engineering
7. Building the Model
8. Evaluation of the Model
9. End Results

# End Results
- After all the possible experiments Maximum accuracy of **92.59%** is achieved by using **XGBoosting Classifier**.
- Here our model correctly predicts whether we should approve Credit Card for Customer or not.
