# Neural_Network_Charity_Analysis

## Purpose
#### The alphabet Soup's business team has funded 34,000 organizations over the years. The purpose of this analysis is to study the data and create a deep neural network model to see the loan prediction risk.

## Results

### Data Preprocessing

The data contains the following columns:

1. EIN and NAME—Identification columns
2. APPLICATION_TYPE—Alphabet Soup application type
3. AFFILIATION—Affiliated sector of industry
4. CLASSIFICATION—Government organization classification
5. USE_CASE—Use case for funding
6. ORGANIZATION—Organization type
7. STATUS—Active status
8. INCOME_AMT—Income classification
9. SPECIAL_CONSIDERATIONS—Special consideration for application
10. ASK_AMT—Funding amount requested
11. IS_SUCCESSFUL—Was the money used effectively

#### What variable(s) are considered the target(s) for your model?
the target variable is the IS_SUCCESSFUL column

#### what variable(s) are considered the features for your model?
The features variables for my model is APPLICATION_TYPE, APPLICATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT.

#### what variable(s) are neither targets nor features and should be removed from the input data?
I removed the EIN and NAME columns.


### Compiling, Training and Evaluating the Model

For the first attempt, I tried to use two rely layer model with 8 neurons for the first layer and 5 neurons for the second layer and sigmoid activation for the output layer. The performance is lower than the target 75% performance.
<img width="622" alt="1" src="https://user-images.githubusercontent.com/92563285/158252334-f1feb1a0-c30b-4ee7-b6c8-a1b25996513c.png">

For the seond attemp, I increased the neurons on both layers by double with same activations on all the layers. The performance is still lower than the target 75% performance.
<img width="609" alt="2" src="https://user-images.githubusercontent.com/92563285/158252620-b2ed4dbb-2cc5-4a95-85f3-cdc6af3417f8.png">

For the third attempt, I tried to increase the neuron for the first layer to 20 with relu activation and 10 neurons for the second rely activation layer and keep the output layer the same. The performance is still lower than the target performance 75%.
<img width="603" alt="3" src="https://user-images.githubusercontent.com/92563285/158252975-04b89035-26ef-4dca-a136-6487587a234d.png">

For the fourth attempt, I changed the number of values for the application_type bin. I used 20 neurons with relu activation for the first layer and 10 neurons with tanh activation for the second layer. The performance is still lower than the 75% target performance. 
<img width="611" alt="4" src="https://user-images.githubusercontent.com/92563285/158253403-e89f63c0-6cb9-4d13-b52b-da72ef4ee5ee.png">

## Summary
I was not able to reach the 75% performance target on all four attempts. The reason for the failure could be I had the wrong activation function type, number of neurons or layers or I did not clean the data correctly.
