# Multiple Linear Regression
## Bike Sharing Case Study

#### Problem Statement:

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.
In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19.

Specifically, company to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
1. Which variables are significant in predicting the demand for shared bikes.
2. How well those variables describe the bike demands

### Steps Performed For multiple linear regression
1.	Reading and understanding the data
    1. Reading data set and its various parameters like no of columns , rows, no of non null values, understanding the numeric plus categorical variables
    2. Visualizing the data – plot graphs to look at visualizations and corelations between variables
2.	Data Preparation
    1. Perform EDA to clean the data , handle the format of data properly.
    2. Create Dummy variables from categorical variable
    3. Append dummy variables and drop originals from the main dataset
    4. Split data into Train and Test (Ratio can be 70-30/80-20)
    5. Rescaling the feature
    6. Look at the correlation among all the variables so that we can select the variables for model building
3.	Building Model :- There two techniques to build the model
    1. Select the model building Technique (forward selection Or backword elimination)
        1. Forward selection :-
            1.	Select one variable at a time and start building model with it.
            2.	Add another feature and rebuild the model. 
            3.	Repeat until we have enough variables that fits our model.
        2.	Backword Elimination
            1. Include all variables at first (can be done manually or by using Automated way like RFE
            2. Build the model and look at the summary
            3. Drop the variables which are insignificant one by one 
4.	Perform Residual Analysis (validating assumption) : - 
    1. Calculate Error Terms (residual points)
    2. Plot distributions of Error Terms 
    3. Check if the distribution is normal with mean 0. 
    4. If distribution is normal we are good for model evaluation
5.	Make predictions on test dataset
6.	Model Evaluation
    1. Calculating r2 for test and comparing with model if similar then the model is good.
    2. Understand the spread for r2

### Conclusions

**1. The variables that are significant in predicting the demand for shared bikes are :-**
1. Registered
2. Casual
3. Holiday 
4. Wednesday 
5. Mist 
6. Feb 
7. yr

**2. How well those variables describe the bike demands :-**
1. Number of registered users are having more impact on bike sharing than number of casual users.
2. Bike shares are high when there is holiday
3. from weekday the bike share is high on wednesday
4. ALso it is an observation that bike share is high when the weather is mist category i.e (Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist)
5. bike shares are also on demand during the Feb Month.


### About Repository (Files) -
1. Python File for MLR assignment named as "Linear Regression Assignment.ipynb"
2. PDF File for Linear regresson Subjective questions with answers.

### Contact
Created by **[@TruptiUD]**
