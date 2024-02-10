# Loan-Eligibility-Prediction-Machine-Learning

Machine Learning Model to predict the loan to be approved or to be rejected for an applicant.

## Introduction:

* In this Loan Status Prediction dataset, we have the data of applicants those who previously applied for the loan based on the property which is Property Loan.
* The bank will decide whether to give a loan for the applicant based on some factors such as Applicant Income, Loan Amount, previous Credit History, Co-applicant Income, etc..,
* Our goal is to build a Machine Learning Model to predict the loan to be approved or to be rejected for an applicant.
* In this project, we are going to classify an individual whether he/she can get the loan amount based on his/her Income, Education, Working Experience, Loan which is taken previously, and many more factors.

Let’s get more into it by looking at the data.

## Data Collection:

* The dataset is collected from Kaggle.
* The data consists of 614 applicant samples and 12 features.
* The 12 features are Loan_ID, Gender, Married, Dependents, Education, Self_Employed, ApplicanIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History and Property Area.

## Feature Engineering:

There are 12 features in the training data. Let's explore the features.

1) Loan_ID-

    * The Loan_ID is generally is used to identify an applicant uniquely but in any way, it doesn’t decide the loan status. So we can ignore the Loan_ID column for the prediction.

2) Gender-

    * Gender is a nominal kind of qualitative data, because there is no numerical relation between different genders.
    * For 13 applicants, Gender is not mentioned in the data.
    * The Unique values are Male and Female
    * There are 489 Male and 112 Female applicants
  
3) Married-

    * Since there are only 2 kind of values are possible to be present in this feature which is married or not married. This is a binary kind of qualitative data.
    * For 3 applicants, Married is not mentioned in the data.
    * The two unique values present in the feature is Yes and No.

4) Education

    * The Education column is a binary kind of qualitative data. Because there are only two values possible in this feature. They are Graduated and Not Graduated.
    * All the applicants given their Education Details
    * The two binary values are Graduate and Not Graduate.

5) Dependents

    * The Dependents feature is a discrete kind of quantitative data.
    * From my thought, dependents feature refer to the number of children of applicant.
    * For 15 applicants, Dependents is not mentioned in the data.
    * There are 4 unique values present in this feature. They are 0, 1, 2, and 3+.
      
6) Self_Employed

    * The Self_Employed column is a binary kind of qualitative data. Because there are only two values possible in this feature. They are Self_Employed and Not Self_Employed.
    * For 32 applicants, Self_Employed status is not mentioned in the data
    * The two binary values are Yes and No.
  
7) Applicant_Income

    * The Applicant Income column is a continuous kind of quantitative data.
    * All the applicants provided their Applicant Income.
  
8) Co-applicant_Income

    * The Co-applicant Income column is a continuous kind of quantitative data.
    * All the applicants provided their Co-applicant Income.
  
9) Loan_Amount

    * The Co-applicant Income column is a continuous kind of quantitative data.
    * For 22 applicants, the LoanAmount are not mentioned in the data.
  
10) Loan_Amount_Term

    * The Loan_Amount_Term column is a discrete kind of quantitative data.
    * For 14 applicants, the Loan_Amount_Term is not included in the data.
  
11) Credit_History

    * It is a binary kind of qualitative data.
    * For 50 applicants, the Credit_History are not mentioned in the data.
    * It consists of binary values.
       * For applicants having Credit_History - 1
       * For applicants aving Credit_History - 0
     
12) Property_Area

    * The Property_Area column is a ordinal kind of qualitative data.
    * All the applicants given their Property_Area.
    * The ordinal datas present in this column are Urban, Semiurban and Rural.
   
## Methodology:

  * Analysed the data for statastical Analysis, Missing Values, Correlational analysis.
  * Found outcome distribution and correlation between input parameters.
  * Split the data into training and testing dataset and further applied normalization.
  * Used support vector machine(SVM) algorithm for prediction.
  * Evaluated models using accuracy score with value of 0.81.
