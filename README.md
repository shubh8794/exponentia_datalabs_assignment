# Exponentia datalabs assignment

**Salary prediction problem:**

We have training data having salary information as categories such as 0to3, 3to6, 6to10 and so on. we have parameters like job experience, job designation, job skills, job summary, job location and company code. 

In order to predict salary of test data we need initial analysis and data cleaning of training data:

**Data cleaning includes:**
1. Drop duplicate values
2. Handle missing values
3. Remove outliers
4. Text cleaning by removing punctuations, numbers and convert all string to lowercase

After this, I converted experience and salary to a fixed number so that it would be helpful in the analysis.

**Steps to build model and re-classification of categories:**

1. Calculate mean salary
2. Create bag of words sparse matrix of the location, skills, designation and summary.
3. Identifying locations, designation and skills that are most popular in above median salary jobs. 
4. Create new columns for each of them and assign binary values based on the presense and absence of them.
5. Drop previous variables corresponding to them and create new matrix of independent variables having columns as experience, good_city, good_desig and good_skills.
6. Convert salary again to categories.
7. We can use classification algorithm for classifying each of record into various classes. 
8. Tried different algorithms like logistic regression, naive bayes and random forest classifier and select one with best score.
9. Using fit parameters of classifier we can predict salary of our text data.


