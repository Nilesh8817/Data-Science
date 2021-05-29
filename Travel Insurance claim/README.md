# Insurance Claim Status Prediction

<p>Insurance companies take risks over customers. Risk management is a very important aspect of the insurance industry. Insurers consider every quantifiable factor to develop profiles of high and low insurance risks. Insurers collect vast amounts of information about policyholders and analyse the data.
As a Data scientist in an insurance company.</p>

This project entails creating a model that can predict for whether a customer can claim for Insurance or not.

## Dataset Description

A file consists of data corresponding to 50552 columns which are 50552 customers and of 12 Features (Columns). Following are the features of the dataset

   - Target: Claim Status (Claim)

   - Gender : 1 - Male, 0 - Female (Gender)

   - Name of agency (Agency)

   - Type of travel insurance agencies (Agency.Type)

   - Distribution channel of travel insurance agencies (Distribution.Channel)

   - Name of the travel insurance products (Product.Name)

   - Duration of travel (Duration)

   - Destination of travel (Destination)

   - Amount of sales of travel insurance policies (Net.Sales)

   - The commission received for travel insurance agency (Commission)

   - Age of insured (Age)

   - The identification record of every observation (ID)

 
Presentation file:<br>

[Travel Insurance claim](Travel_Insurance_Claim.ipynb)

## Evaluation Metric

The evaluation metric for this task will be `precision_score`. Read up about it more [here](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html).

________________________________________________________________________________________________________________________________________________________________

## EDA and Preprocessing

### Null values in %

<img src="plots/null.png">

<p> Dropped Gender and ID column </p>

## Analyze Categorical columns


<p> Dropped Dristribution channel (Highly imbalanced) and Destinations (Too many classes) </p>

## Analyze Numerical columns

<p> Replaced duration values < 0 with average duration of their respective destination </p>   

## Bivariate Analysis against the traget

## Baseline model

<p> Decision Tree Classifier</p>

<img src="plots/report1.png">

### Recall for class 1 is 0.71, that means out of all the claims which should be approved, 71% is predicted accurately.

