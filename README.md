# Module 21 Challenge - Deep Learning Challenge

## Background

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

* **EIN and NAME** — Identification columns
* **APPLICATION_TYPE** — Alphabet Soup application type
* **AFFILIATION** — Affiliated sector of industry
* **CLASSIFICATION** — Government organization classification
* **USE_CASE** — Use case for funding
* **ORGANIZATION** — Organization type
* **STATUS** — Active status
* **INCOME_AMT** — Income classification
* **SPECIAL_CONSIDERATIONS** — Special considerations for application
* **ASK_AMT** — Funding amount requested
* **IS_SUCCESSFUL** — Was the money used effectively

## Results Summary
My attempts at optimizing the model resulted in a slight success. The accuracy of the model was initially 72.63% and improved to 74.03% upon my second attempt at optimization. This improvement in optimization was only possible for me to obtain if I do not drop the NAME column while optimizing the model. Despite this making the training step of the model very slow, there seems to be a correlation between the name of the organizations and the rate of success so it was worth trying to include in the training. No matter how much I modified the number of values for each bin, the number of hidden layers, or number of epochs to the training regimen, the accuracy never changed more than a couple fractions of a percent until I trained with the NAME column included.