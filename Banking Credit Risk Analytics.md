# Bank Loan Analysis Dashboard
---
## Overview
Banks make the most profit when they lend money to borrowers who later pay it back with interest. In this case, Thera Bank has more depositors who are considered as liability customers. The number of customers who borrow is small, and Thera Bank seeks to expand its profit base by onboarding more loan businesses. The bank intends to explore ways to convert liability customers to asset customers(borrowers) while still retaining them as depositors. 
## Data Sources
The dataset used for this project is "Bank_Personal_Loan_Modelling" [View the data](https://docs.google.com/spreadsheets/d/1z7fKyO-uF3QNCckzdc2JMztCp0lXr62s/edit?usp=sharing&ouid=116799710055860433651&rtpof=true&sd=true).

The data contains two sheets:
  1. Description - contains a brief description of the columns in the data.
  2. Data 
## Tools
This project was done in: 
- *Power BI Desktop* [Download Here](https://www.microsoft.com/en-us/download/details.aspx?id=58494)
- *Power Query*
## Data Cleaning and Preparation

A custom column, 'Mortgage_Flag', was added where an M language was written.
```M
if morgage = 0
then 0
else 1
```
The original mortgage column was then deleted. 
## Exploratory Data Analysis
- What is the personal loan rate?
- What percentage of customers have a CD account? 
- What is the average income?
- How does credit card spending relate to taking a personal loan?
- How does education affect the personal loan rate?
- What is the correlation between average income and personal loans?
- How do credit spending, CD accounts, and personal loans correlate?
## Data Analysis
- Personal Loan Rate
 ```dax
Personal Loan Rate = DIVIDE(
                            SUM(Data[Personal Loan]),
                                COUNT(Data[Personal Loan])
                           )
```
![image](https://github.com/user-attachments/assets/85fda492-e6cf-481e-853d-461b79b1715f)

- Personal Loan Rate vs Education
  
  
- Personal Loan Rate vs Family Size
![image](https://github.com/user-attachments/assets/ec41049c-340d-4fc6-9869-57c3160b794e)

- Personal Loan Rate vs Mortgage
![image](https://github.com/user-attachments/assets/f405ee7c-4fce-4210-b999-6b3dfe251fbd)

- Personal Loan Rate vs Securities Account
![image](https://github.com/user-attachments/assets/8345e644-007f-4e6d-b724-f417e2541627)

- Personal Loan Rate vs Deposit Account
![image](https://github.com/user-attachments/assets/feb51d40-72ac-4d6c-98c3-8dea6e23b0bd)

## Results and Findings

## Recomendation
