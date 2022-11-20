# Udacity project 4

## Project motivation

This project is the final project from Udacity Data science Nanodegree. In this project I was interested in providing an analysis on a simulated dataset 
containing data about Starbucks offers sent to its clients. Using the given data I set a goal to provide a reaserch/modelling on the following:

- How does the population of Starbucks customers look like? E.g. age, gender, income distribution. 
- How Various age, income, gender etc. groups of customers responded to the offers send to them?
- Build a model that predicts how likely a given customer is to respond to the offer send to him/her.

## Installation and libraries

The code used for this project is written python 3.7. I used the following libraries:

- pandas
- numpy
- math 
- json
- seaborn
- sklearn
- xgboost
- matplotlib

## Files description

In this repository there are the following files:

- starbucks.ipynb - Jupyter notebook with the analysis code
- README.md - Readme file
- data - directory containg json files with data used for the analysis. Contains the following files.
  - profile.json
    Rewards program users (17000 users x 5 fields)
      
     - gender: (categorical) M, F, O, or nul
     - age: (numeric) missing value encoded as 118
     - id: (string/hash)
     - became_member_on: (date) format YYYYMMDD
     - income: (numeric)
        
   - portfolio.json
   Offers sent during 30-day test period (10 offers x 6 fields)

     - reward: (numeric) money awarded for the amount spent
     - channels: (list) web, email, mobile, social
     - difficulty: (numeric) money required to be spent to receive reward
     - duration: (numeric) time for offer to be open, in days
     - offer_type: (string) bogo, discount, informational
     - id: (string/hash)
        
   - transcript.json
   Event log (306648 events x 4 fields)

     - person: (string/hash)
     - event: (string) offer received, offer viewed, transaction, offer completed
     - value: (dictionary) different values depending on event type
     - offer id: (string/hash) not associated with any "transaction"
     - amount: (numeric) money spent in "transaction"
     - reward: (numeric) money gained from "offer completed"
     - time: (numeric) hours after start of test
        
## Results

Some results from the analysis which I provided :

- People who described their gender as 'other' are the most responsive to offers send to them.
- Male customers are more likely to respond to the offers than female.
- The older is the customer the more likely he is to respond to the offer.
- The richer is the customer the more likely he is to respond to the offer.

## Acknowledgements

Acknowledgements to udacity for the idea of the project and for Starbucks for sharing their data.

## External links

Main findings of the code can be found in the medium post located [here](https://medium.com/@tomekfaber_55869/predicting-offers-sent-to-starbucks-customers-a04b031d0314) 
        
