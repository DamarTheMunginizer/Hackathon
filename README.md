---
title: Data Science Venn Diagram
type: exercise
creator:
    name: Alexander Combs
    city: NYC
---

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)  Data Science Venn Diagram

Today we are going to have a team-based competition. The goal is to create the best performing model on a hold-out sample of data. Simple right?

Well, there is a catch.

This will be a constrained optimization. To understand what that means, let's take a look at the Project Management Venn Diagram, below.

![](https://www.pyragraph.com/wp-content/uploads/2013/04/GOOD-FAST-CHEAP.jpg)

The idea is that for any project, you can have two of these. 
- You can have good work done cheap, but it will take a long time. 
- You can have good work done fast, but it won't be cheap.
- Or you can have work done fast and cheaply, but it won't be good.

Today we will apply this concept to data science. You will be given a dataset and teams will be randomly assigned to one constraint: samples, features or algorithm.

---

### Team Sample Constraint
- Your choice of algorithm
- Your choice of features
- **Must use the cheap train sample**

### Team Features Constraint
- Your choice of algorithm
- **Limited to a maximum of 20 features**
- Your choice of samples

### Team Algorithm Constraint
- **Must use a Random Forest**
- Your choice of features
- Your choice of samples

# ![](https://media.giphy.com/media/aL4bDxt8fbpy8/giphy.gif)
 
 ### Submission
 
The task is to predict if a person's income is in excess of $50,000 given certain profile information. 

For your submission, you **must**:
1. Generate the predicted probability that a given person's income will be **above** $50,000 for each row in the test set.
2. Place these predicted probabilities in a single .csv file. Your .csv file should have _exactly_ one column named **`wage`**.
3. Use the below Google form to submit before 2:30 p.m. Eastern time.

#### [Submission Link](https://docs.google.com/forms/d/e/1FAIpQLSeKSkyg8x4UEKy1pcDqLEPiKJk184lTQvNVLaIdWnbg4Kh4eA/viewform?usp=sf_link)

Good luck!

#### [Data Description]
| Variable Name  | Role    | Demographic     | Description |
|----------------|---------|-----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| age            | Feature | Age             | N/A                                                                                                                                                                                                                                                                                                                                                                                                                             |
| workclass      | Feature | Income          | Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.                                                                                                                                                                                                                                                                                                                          |
| fnlwgt         | Feature |                 |                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| education      | Feature | Education Level | Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.                                                                                                                                                                                                                                                                          |
| education-num  | Feature | Education Level |                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| marital-status | Feature | Other           | Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.                                                                                                                                                                                                                                                                                                                      |
| occupation     | Feature | Other           | Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.                                                                                                                                                                                                       |
| relationship   | Feature | Other           | Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.                                                                                                                                                                                                                                                                                                                                                             |
| race           | Feature | Race            | White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.                                                                                                                                                                                                                                                                                                                                                                    |
| sex            | Feature | Sex             | Female, Male.                                                                                                                                                                                                                                                                                                                                                                                                                   |
| capital-gain   | Feature |                 |                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| capital-loss   | Feature |                 |                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| hours-per-week | Feature |                 |                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| native-country | Feature | Other           | United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands. |
| income         | Target  | Income          | >50K, <=50K.                                                                                                                                                                                                                                                                                                                                                                                                                    |
