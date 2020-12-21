# Finding_donors
A Charity organization wants to know which factors impact the income of a person.A general trend has been observed that person with income greater then 50k is more likely to donate.
Now company wants to develope a machine learning infrastructure to target their advertisment and campaigns toward only those person that have income greater then 50k.Company also wants to know which factors impact the income of a person in order to make their advertisment more targeted.
### Data

The modified census dataset consists of approximately 32,000 data points, with each datapoint having 13 features. This dataset is a modified version of the dataset published in the paper *"Scaling Up the Accuracy of Naive-Bayes Classifiers: a Decision-Tree Hybrid",* by Ron Kohavi. You may find this paper [online](https://www.aaai.org/Papers/KDD/1996/KDD96-033.pdf), with the original dataset hosted on [UCI](https://archive.ics.uci.edu/ml/datasets/Census+Income).

**Features**
- `age`: Age
- `workclass`: Working Class (Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked)
- `education_level`: Level of Education (Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool)
- `education-num`: Number of educational years completed
- `marital-status`: Marital status (Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse)
- `occupation`: Work Occupation (Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces)
- `relationship`: Relationship Status (Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried)
- `race`: Race (White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black)
- `sex`: Sex (Female, Male)
- `capital-gain`: Monetary Capital Gains
- `capital-loss`: Monetary Capital Losses
- `hours-per-week`: Average Hours Per Week Worked
- `native-country`: Native Country (United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands)

**Target Variable**
- `income`: Income Class (<=50K, >50K)

# Getting started
First we will download required dependencies to get started with this project
```
pip install numpy
pip install sklearn
pip install matplotlib
```
# Outcome
Major purpose of this project is to develop a machine learning algorithm for a ficticious charity organization.We will develop a model that will allow company to predict wether a certain user have income greater then 50K USD or less.If a person have income greater then 50K Usd this means that person possibly can have enough money to donate to our organization.    
Choose a scikit-learn classifier (e.g., adaboost, random forests) that has a feature_importance_ attribute, which is a function that ranks the importance of features according to the chosen classifier. In the next python cell fit this classifier to training set and use this attribute to determine the top 5 most important features for the census dataset.    
<img src="Capture.PNG" width=750px>  

# Summary
So what did we do? We got a data set and we set a target to classify people that make more than $50,000 annually. We cleaned the data, normalized and converted the necessary variables into numerical features so that we can use them in our models. We shuffled and split our data into training and testing sets. We set a baseline predictor and built three other models. We chose the ADABOOST model as the best choice. We tuned it further and made it slightly better. We tried to use the model with only the five main features but it performed slightly worse. 


# Usage Example
Our main code in written in a well documented notebook that explains everything perform data acquistion to data preprocessing and eventually data modelling with various contraints.
However here are some usage examples,
```
bestclf.predict(X_train)
```
where X_train is a set of features on which our data will make predictions in following order.   
   

# License
This project is licensed under [MIT License]('https://choosealicense.com/licenses/mit/')
Now your setup is ready for running this project.
