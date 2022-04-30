[<img src="https://img.shields.io/badge/Linkedin-%230A66C2.svg?&sflat&logo=linkedin&logoColor=white" alt="Linkedin profile link button" height="20" width="70" />](https://www.linkedin.com/in/melodyyip/) &emsp;[<img src="https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white" alt="View in Medium" height="20" width="70" />](https://medium.com/@melodyyip515_/titanic-survival-prediction-using-machine-learning-89a779656113) &emsp;[<img src="https://img.shields.io/badge/Tableau-%23ff4d4d.svg?&sflat&logo=tableau&logoColor=white" alt="Tableau profile link button" height="20" width="70" >](https://public.tableau.com/app/profile/yip.hoi.ching#!/?newProfile=&activeTab=0) &emsp; [<img src="https://img.shields.io/badge/Github Blog-%23181717.svg?&style=flat&logo=github&logoColor=white" alt="Github profile link button" height="20" width="90" alt="Github Blog Button"/>](https://melodyyip.github.io/RFM_UCLonlineStore/) 

# Titanic_survival_prediction_ML
Titanic Survival Prediction Using Machine Learning

### Challenge
Predict whether a passenger on the titanic would have been survived or not

### Data

![alt text](https://miro.medium.com/max/606/1*ItbI-LwOHTHLgRtKUYK_Zg.png)


### Workflow stages

The competition solution workflow goes through seven stages described in the Data Science Solutions book.
1. Question or problem definition
2. Wrangle, prepare, cleanse the data
3. Exploratory Data Analysis
4. Acquire training and testing data
5. Model, predict and solve the problem

### 1. Question or problem definition

The competition is simple: Use the Titanic passenger data (name, age, price of ticket, etc.) to try to predict who will survive and who will die. This is a binary classification.

Binary classification is the task of classifying the elements of a set into two groups on the basis of a classification rule.

The values in the second column (“Survived”) can be used to determine whether each passenger survived or not:
if it’s a “1”, the passenger survived.
if it’s a “0”, the passenger died.


### 2. Wrangle, prepare, cleanse the data
Here is my workflow for cleaning the data. I am not going to show all the step here, you can check my Kaggle for full code. Check my Kaggle and GitHub to took a look at all my projects🍀

### 3. Exploratory Data Analysis
Analyze, identify patterns, and explore the data Analysis
![alt text](https://miro.medium.com/max/630/1*xzS2rilv6HeCRGVx8CN_bQ.png)

Only 350 out of 891 passengers (38.4%) survived in the training set.
![alt text](https://miro.medium.com/max/630/1*y8pxlriPY1hXTGQIuuPhzQ.png)

#### Sex
The number of men on board the ship is much higher than the number of women, but the number of women saved is more than twice that of the number of males survived.
The survival rates for a women on the ship is around 75% while that for men in around 19%.

#### Pclass
Passenegers Of Pclass 1 has a very high priority to survive.
The number of Passengers in Pclass 3 were a lot higher than Pclass 1 and Pclass 2, but still the number of survival from Pclass 3 is low compare to them
Pclass 1 %survived is around 63%, for Pclass2 is around 48%, and Pclass3 survived is around 25%


Sex and class are important factors for survival. Let’s determine survival rate based on sex and class together

![alt text](https://miro.medium.com/max/630/1*vHkwpb8ZtVpbv8OXtOVlGQ.png)
- Female from Upper class is about 95–96% survived. Only 3 out of 94 Women from Upper class died.
- Female Upper class has high priority to survive
- Lower class female has more survived rate than Upper class male


#### Features Correlation with Survived:

![alt text](https://miro.medium.com/max/453/1*udZOU1paiDFpkmZK_xQaTw.png)


- Sex is positively corrlated with Survived (with a Person’s correlation coefficient of 0.54) ; Female is more likely to survive
- Pclass is negatively correlated with Survived(with a Pearson’s correlation coefficient of -0.34) ; Obviously, better the ticket class (1 = 1st/Upper ; 2 = 2nd/Middle; 3 = 3rd/Lower), higher the chance of survival.
- Those important feature for prediction the Survived people

### 4. Acquire training and testing data
 Check my Medium to took a look at this part🍀

### 5. Model, predict and solve the problem
Check my Medium to took a look at this part🍀

### Model selection
![alt text](https://miro.medium.com/max/229/1*OBZ5ZA6HCnhZhM_VpSdzDg.png)

Random Forests and Decision Trees are the most accurate (96.97%) in predicting the survival of passengers and they are select to predicted the testing data.

#### Visualize the decision tree
![alt text](https://miro.medium.com/max/630/1*hkm5PkA8ITsM5ODKv7LzwA.png)

#### Finding :
According to the analysis, passengers were more likely to survive if:
- Upper class ticket
- Women/Lady
On the contrary, being a Lower class old man lowered the chances of survival.
Give me a clap if you find my article is useful.👏👏👏
