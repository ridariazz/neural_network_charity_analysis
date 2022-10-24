# Overview 

The purpose of this analysis was to work with neural networks. Our knowledge of machine learning and neural networks we created a binary classifer that's capable of predicting whether the applicants will be successful if funded by Alphabet Soup. We are working with a CSV file that contains more than 34,000 organizations that have recieved funding from Alphabet Soup over the years. 

Within this dataset are a number of columns that capture metadata about each organization, such as the following:

- EIN and NAME—Identification columns

- APPLICATION_TYPE—Alphabet Soup application type

- AFFILIATION—Affiliated sector of industry

- CLASSIFICATION—Government organization classification

- USE_CASE—Use case for funding

- ORGANIZATION—Organization type

- STATUS—Active status

- INCOME_AMT—Income classification

- SPECIAL_CONSIDERATIONS—Special consideration for application

- ASK_AMT—Funding amount requested

- IS_SUCCESSFUL—Was the money used effectively

# Results 

## Data Preprocessing

1. What variable(s) are considered the target(s) for your model? 

Variable that is considered as the target for our model is the IS_SUCCESSFUL column which indicates that is has been successfully funded by the organization. 

2. What variable(s) are considered to be the features for your model?

IS_SUCCESSFUL column 

3. What variable(s) are neither targets nor features, and should be removed from the input data?

We dropped the EIN and NAME columns as they have no impact on our overall outcome 

## Compiling, Training, and Evaluating the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?

For my model, I had chosen four layers:

- First layer: 110 neurons 

- Second layer: 80 neurons 

- Third layer: 20 neurons 

- Fourth layer: 1 neuron 

For our analysis, it seems sigmoid was the better fit for layers 3 and 4 while relu activation was better for layers 1 and 2. 

(add model 2 image)

2. Were you able to achieve the target model performance? 

The target for the model is 75%, but we weren't able to reach that percentage. Our non-optimzation model's accuracy was 68.4%. Moreover, to improve our model's accuracy performance, we increased the accuracy to 72.5% in the optimzation analysis. However, we were unable to achieve the target model performance from both models. 

(model 1 accuracy)

(model 2 accuracy)

3. What steps did you take to try and increase model performance?

Went ahead and dropped more columns on our second analysis **'EIN','NAME','STATUS','USE_CASE'.** Also, I added 2 additional layers to the mode and it seems sigmoid as well as relu pair well together. By doing so, the model accuracy went up from 68.4% to 72.5%

(model 1 neurons) 

(model 2 neurons)

(model 2 columns)

# Summary 

By adding 2 more layers to our model and removing some other unwanted columns that were going to have little to no impact on our overall analysis, we were able to increase our accuracy to 72.5% compared to our first evaluation. Moreover, the relu and sigmoid activations yielded a higher accuracy. 

Another model that can solve this classification problem is the **Random Forest Classifier** as it's a supervised learning technique that combines a number of decision trees on different subsets of a dataset. Moreover, it averages the results to increase the dataset's predicted accuracy and is less influenced by outliers. 