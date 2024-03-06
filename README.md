# Lending Club Case Study
This case study involves peforming Exploratory Data Analysis (EDA) on the data set provided for approved loans. The main objective is to identify patterns of loan defaulters and the factors that are influencing them. Various loan attributes such as interest rate, customer demographics, loan amount, income of the borrowers etc are considered for the analysis.


## Table of Contents
* [Objective](#Objective)
* [Data Set Analysis] (#datasetanalysis)
* [Approach] (#approach)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [Contacts] (#contacts)

## Objective
  The primary objective of the case study is to identify patterns which causes loans to get defaulted.  By analyzing the attributes provided in the dataset, we attempt to gain insights into what the major factors are for defaulting that would assist Lending Club from making informed decisions while approving future loan applications thereby reducing the amount of credit loss.

## Data Set Analysis
 Data set provided on the past loan approvals containted many attributes including whether the borrower defaulted or not, loan amount, approved amount, date of approval, address, employment tenure, dti, verification status etc. 

 ### Approach

 The data set was analysed and we took the following approach for our analysis:

 1. Data Cleansing: By looking a the data, we applied the following techniques to keep only relevant data for our analysis

    a. There were no summary or total rows and hence all rows were initially considered
    b. Identified columns that have more than 70% of null values and removed them from the data set
    c. All irrelevant columns for this analysis have been identifed and removed 
    d. The id and member_id columns which only contained the unique values were also removed from the analysis
    e. Removed extra spaces on Term (term) column and removed % character on the Interest Rate(int_rate) column and converted as float
    f. Added a new column to store Year from the loan issued date (issue_d) column 

 2. Identifying Key attributes that contribute to analysis
 
    The key driving categorical variable we identified is the loan_status column which has three possible values:
        - Fully Paid - The Loan has been paid up and closed
        - Current - The loan is still being paid
        - Charged Off - Loan is not paid entirely and is defaulted

    Our Analysis centered around this column against the other attributes to identify possible causes of loan default.

3. Univariate Analysis: Univariate analysis were performed on the Term and Year columns to understand how the data is distributed

4. Bi/Multivariate Analysis: To explore relationship of loan status columns with other attributes such as Year, Interest Rate, Grade, Home Ownership, Verification Status, Purpose of loan, State of residence, dti and loan amount were performed to identify patterns for default.

5. Visualizations: For each of the anlaysis performed, histogram, bar, boxplot and line graphs were plotted to identify likelihood of laon defaulters

6. Insights: Based on these, we came up with insights as to what are the top attributes that contribute most for loan defaulting.
   

## Conclusions
- Lending Club as a company has grown over the years. They approved more number of loan applications every year. Along with it, the defaulter numbers have grown as well
- People seems to default more on 36 term loans who have said debt consoliation as their purpose. LC can put some stringent contols in place when people apply for loans in this category
- LC can consider having higher interest rates for high risk loans. 
- The company should also adhere to strict verification process and ensure Source Verification is completed before issuing loans. This would certains help reduce their losses.
- Finally, they should perform higher due deligence when it comes to residents of CA, NY and FL while approving loans


## Technologies Used
- python 3.11.5
- numpy 1.24.3
- pandas 2.0.3
- matplotlib 3.7.2
- seaborn 0.12.2
- Jupyter Notebook 6.5.4
- Google Colab



## Acknowledgements
References
  - stackoverflow and geekforgeek websites for python examples
  - Understanding domain knowlege about credit risk analysis
       - Finbox -->  https://finbox.in/blog/credit-risk-analysis/#:~:text=Credit%20Risk%20Analysis%20is%20evaluating%20a%20borrower%27s%20ability,the%20level%20of%20risk%20involved%20in%20extending%20credit.
       
   - Understanding debit to income ratio
        - CFI --> https://corporatefinanceinstitute.com/resources/commercial-lending/credit-risk-analysis-models/
   - What is EDS by Prasad Patil -->  https://towardsdatascience.com/exploratory-data-analysis-8fc1cb20fd15
   - Course materials from upGrad curriculam


## Contacts
  Manikandan Krishnamurthy Vembu and Deepenti Jha (https://github.com/manikvgithub)

