# Employee Promotion - Machine Learning 2023

Content:

A large MNC have 9 broad verticals across the organisation. One of the problem is identifying the right people for promotion (only for manager position and below) and prepare them in time.

The final promotions are only announced after the evaluation and this leads to delay in transition to new roles. Hence, company needs help in identifying the eligible candidates at a particular checkpoint so that they can expedite the entire promotion cycle.

Multiple attributes have been provided around Employee's past and current performance along with demographics.

Features:

employee_id: Unique ID for employee
department: Department of employee
region: Region of employment (unordered)
education: Education Level
gender: Gender of Employee
recruitment_channel: Channel of recruitment for employee
no_ of_ trainings: no of other trainings completed in previous year on soft skills, technical skills etc.
age: Age of Employee
previous_ year_ rating: Employee Rating for the previous year
length_ of_ service: Length of service in years
awards_ won?: if awards won during previous year then 1 else 0
avg_ training_ score: Average score in current training evaluations
is_promoted: (Target) Recommended for promotion

About project
We will predict whether an employee will be promoted or not. The steps that we will take include:

- <ins><b>Data Preprocessing:</b></ins> the dataset will be preprocessed by removing irrelevant columns, handling missing values, 
and cleaning the text data by removing stop words, punctuation, and special characters;
- <ins><b>Exploratory Data Analysis (EDA):</b></ins> EDA will be performed to understand the distribution of fake and real news
articles in the dataset;
- <ins><b>Model Selection:</b></ins> for model selection we will use some supervised algorithms and also deep learning. Supervised
models that we will use include: Linear Regression, Random Forest, Decision Tree, Naive-Bayes, Support Vector 
Machines (SVMs);
- <ins><b>Model Evaluation:</b></ins> we will evaluate the performance of the trained model on the testing data using metrics such as 
accuracy, precision, recall, and F1-score.

