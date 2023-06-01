<h1> <b>Employees Promotion Prediction - Machine Learning 2023</b> </h1>

As part of Machine Learning project we will use an HR Dataset containing employees data taken by <a href="https://www.kaggle.com/datasets/arashnic/hr-ana">Kaggle</a>. </br>
While using the dataset above we are trying to predict if an employee will be promoted or not and what are the factors that have an impact in employee promotion by using Machine Learning Algorithms.


**Project steps that we will take:**

<ul>
<li>Exploratory Data Analysis (EDA):
    <ul>
      <li>EDA will be performed to understand the distribution of promoted employees;</li>
    </ul> 
  </li>
  <li>Data Preprocessing:
    <ul>
      <li>The dataset will be preprocessed by removing irrelevant columns, handling missing values, checking for outliers and more;
      </li>
    </ul>
  </li>  
  <li>Model Selection:
    <ul>
      <li>For model selection we will use some supervised algorithms and also deep learning. Supervised models that we will use include: Logistic Regression, Random Forest (RF), Decision Tree, Naive-Bayes, Support Vector Machines (SVMs), K-Nearest Neighbor (KNN)</li>
    </ul>
  </li>
  <li>Model Evaluation:
    <ul>
      <li>We will evaluate the performance of the trained model on the testing data using metrics such as accuracy, precision, recall, and F1-score.</li>
        <li>We will try the 80/20 train_test_split and see if the accuracy gets better.</li>
      <li>There will be a comparison between models both in a table form and graph form.</li>
      <li>For the best performing algorithms we will check for the most import features.</li>
      <li>We will do some real life examples regarding the employee promotion.</li>
    </ul>
  </li>
</ul> 
<hr>

<h5>Results </h5>
<p> Accuracy for 0.2 and 0.3</p>

Model  | 80/20  | 70/30 
------------- | -------------  | -------------
Logistic Regression  | 0.6787495013960909   | 0.6821233878473607
Random Forest  | 0.9419126445951336   | 0.9371426671985108
Decision Tree  | 0.7953230953330674   | 0.8139875016620131
Naive Bayes  | 0.6688272836059035   | 0.6703230953330674
SVM  | 0.7039289988033506   | 0.7092806807605372
K-Nearest Neighbor  | 0.7040287195851616   | 0.699707485706688

<p> Train accuracy for 0.2 and 0.3</p>

Model  | 80/20  | 70/30 
------------- | -------------  | -------------
Logistic Regression  | 0.6834737734343838   | 0.6803806484699982
Random Forest  | 0.9950762863980853   | 0.9953131232548863
Decision Tree  | 0.999   | 0.9994
Naive Bayes  | 0.6808   | 0.667
SVM  | 0.7424   | 0.738
K-Nearest Neighbor  | 0.8062   | 0.8108

<p> Test accuracy for 0.2 and 0.3</p>

Model  | 80/20  | 70/30 
------------- | -------------  | -------------
Logistic Regression  | 0.6787495013960909   | 0.6821233878473607
Random Forest  | 0.9419126445951336   | 0.9371426671985108
Decision Tree  | 0.7953230953330674   | 0.8139875016620131
Naive Bayes  | 0.6688272836059035   | 0.6703230953330674
SVM  | 0.7039289988033506   | 0.7092806807605372
K-Nearest Neighbor  | 0.7040287195851616   | 0.699707485706688

<p> From the results we can see that:</p>
<ul>
    <li>Random Forest and Decision Tree have performed the best in both ratios</li>
    <li>Naive Bayes has performed the worst in both ratios.</li>
    <li>The accuracies in both ratios show similar values. Some algorithms performed better with 0.3 such as: DT and RF and the other ones performed better with 0.2. This could mean different things like:
        <ul>
            <li>DT and RF tend to have higher model complexity and are more prone to overfitting. With a larger training set, these algorithms may have more data to learn from and can capture more intricate patterns in the data, resulting in better accuracy.</li>
            <li>The train-test split can affect the distribution of data between the training and testing sets. Some algorithms may perform better when trained on a larger portion of the data, while others may benefit from a more balanced representation of the data in the test set.</li>
            <li>The train-test split is often performed randomly, and the particular split can introduce some level of randomness. As a result, different train-test splits can lead to different performance outcomes for the algorithms</li>
        </ul>
    </li>
</ul>


<p> Calculating feature importance for best permorming algorithms </p>

<p> Ranform Forest: </p>

Feature  | Importance  
------------- | -------------  
previous_year_rating  | 0.282231   
avg_training_score  | 0.225695   
age  | 0.146223   
region  | 0.126820   
department  | 0.078141   
recruitment_channel  | 0.050082   
no_of_trainings  | 0.033952   
gender  | 0.029571   
education  | 0.022830   
awards_won  | 0.004457   
length_of_service  | 0.000000 

<p> Decision Tree: </p>

Feature  | Importance  
------------- | -------------  
previous_year_rating  | 0.382249   
avg_training_score  | 0.210603   
age  | 0.119504   
region  | 0.118463   
department  | 0.063634   
recruitment_channel  | 0.040085   
gender  | 0.023273   
no_of_trainings  | 0.023181   
education  | 0.015775   
awards_won  | 0.003233   
length_of_service  | 0.000000 

<p>From the results of both algorithms we can see that:</p>
<ul>
    <li>The most important feature or attribute is previous_year_rating and this shows that previous_year_rating plays the biggest role in getting a promotion.</li>
    <li>avg_training_score is also somewhat an important feature or attribute to employee promotion.</li>
    <li>length_of_service is the feature or attribute that doesn't help in getting a promotion at all. This means that the amount of time you stay in a company doesn't indicate that you will get a promotion without doing a good work.</li>
</ul>

<p>We also did some questions related with this dataset and got interesting results:</p>

<h3>Q1. Do older employees get more promotion than younger employees?</h3>
<p>Youngest age is 20 and oldest age is  60.</p>
<p>Total number of young employees is: 18118  and the total number of young employees promoted is: 1550
Percentage of young employees promoted: 8.56%
Total number of old employees is: 36690  and the total number of old employees promoted is: 3118
Percentage of old employees promoted: 8.50%</p>

<h3>Q2. What is the probability to get promoted, if an employee has won an award?</h3>
<p>Total number of award winning employees is: 1270  and the total number of award winning employees promoted is: 559
Probability of promotion for award-winning employees: 44.02%</p>

<h3>Q3. What is the average training score of those employees who got promoted?</h3>
<p>The Average Training Score for the Employees who got Promotion is 71</p>

<h3>Q4. What is the impact of gender in promotions?</h3>
<p>Female employees: 16312
Male employees: 38496
Male Promoted: 3201
Female Promoted: 1467
Percentage of female promoted employees is: 8.99%
Percentage of male promoted employees is: 8.32%</p>

<h3>Q5. What is the probability that a young and new employee will be promoted?</h3>
<p>Total number of award winning employees is: 1270  and the total number of award winning employees promoted is: 559
Probability of promotion for award-winning employees: 44.02%</p>

<hr>
<h5> Technologies </h5>
<ul> 
    <li> Google Colaboratory </li>
    <li>Languages:
        <ul><li>Jupiter Notebook</li></ul></li>
</ul>
<hr>

<h5>Creators</h5>
<ul>
    <li>Ariana Kadriu</li>
    <li>Edona Pllana</li>
</ul>
<hr>
<h5>Setup</h5>
<ul>
    <li>Import 'employee_promotion.ipynb' file into Google Collaboratory or add it from this repository;</li>
    <li>Upload the used dataset 'employee_promotion.csv' which can be downloaded by <a href="https://www.kaggle.com/datasets/arashnic/hr-ana">Kaggle</a>;</li>
    <li>Then, Runtime > Run All in collaboratory to run the nootebook.</li>
