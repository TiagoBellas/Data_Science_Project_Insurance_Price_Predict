# Insurance-Price-Predict

## Overview

This is a Academic project which aims to develop a machine learning model that accurately predicts insurance prices based on various customer features. By leveraging a dataset containing information about customers and their insurance claims, we aim to provide a reliable tool for predicting future insurance costs.

DATASETS
 - File autodata.txt
 - File claimsdata.txt

TOOLS: Software R Project / Python

## Problems

Insurance companies need to predict the price of premiums for new customers accurately. By analyzing historical data, we can build a model that helps in estimating these prices.

#### Part I

1. Perform a descriptive statistical data analysis of the Number of Claims of the Third Party Liability on Automobile Insurance. Comment on the features observed and highlight values or patterns that you think are important to characterize the phenomenom.

2. Perform a descriptive statistical data analysis of Claims Severity of the Third Party Liability
on Automobile Insurance. Comment on the features observed and highlight values or patterns
that you think are important to characterize the phenomenom.

3. Fit distributions to the Number of Claims and Claim Severity.
  - For the Number of Claims, remove the highest outlier from data. Refer that fact on your
report.
  - For Claims Severity, choose an upper bound that allows you to fit a distribution of the
Exponential Family. Refer, on your report, the upper bound considered and the number
of claims removed from data and give a comment on the choice of the upper bound.
  - What is the mean value and standard deviation of the claims removed from data in question
3? Plot the removed data in a histogram and a boxplot. Comment. Give your opinion on
how should the insurer include that data on the final premium structure.

You are now asked to propose a Pricing Structure for the Automobile Insurance portfolio.
Using all the results from Part I, you are asked to answer the following questions:

#### Part II

Now asked to propose a Pricing Structure for the Automobile Insurance portfolio.
Using all the results from Part I, we are asked to answer the following questions:

1. Fit a GLM to the Number of Claims data and estimate the claim frequency for each risk profile
in your portfolio.
  - Detail and justify your model assumptions and choices.
  - Improve your model, using adequate statistical tests.
  - Evaluate and comment on the quality of the model.
  - Identify the Standard Insured characteristics and the correspondent claim frequency estimate.
  - Include any comments you consider relevant.

2. Fit a GLM to the Claim Costs of “common” claims.
 - Be clear about your definition of “common” claim.
 - Detail and justify your model assumptions and choices.
 - Improve your model, using adequate statistical tests.
 - Evaluate the quality of the model.
 - Include any comments you consider important.

3. Propose a Pricing Structure to the “common” claims. Identify the highest and lowest insured’s
risk profile and the correspondent premiums to be charged. Compare with the premium of the
standard insured.

5. Propose a model that allow you to include the large claims in the Pricing Structure. We may
choose some Machine Learning model that, accurately predicts the probability of reporting a
large claim. Justify your choice.

## Dataset
The dataset used in this project includes customer information and also contract claims information.

- **Automobile Portfolio (file autodata.txt)**: This document provides a summary of the `autodata.txt` file used in the Automobile Portfolio project. The dataset contains various attributes related to automobile insurance policies, which are essential for analyzing and predicting insurance risks and premiums.
-  **Claims Data (file claimsdata.txt)**: This document provides a summary of the `claimsdata.txt` file used in the Claims Data project. The dataset includes key attributes related to insurance claims, focusing on 3rd Party Liability Coverage.

## Data Dictionary

### Automobile Portfolio (file autodata.txt) | Attributes

- **ncontract**: Number of contracts
- **exposition**: Risk Exposition of each policy during the year
- **zone**: Zone of Residence. Classification according to the number of inhabitants per km²
  - A: 1 to 50 inhabitants per km²
  - B: 51 to 100 inhabitants per km²
  - C: 101 to 500 inhabitants per km²
  - D: 501 to 2000 inhabitants per km²
  - E: 2001 to 10000 inhabitants per km²
  - F: More than 10000 inhabitants per km²
- **power**: Power of the vehicle. Classification in categorical levels.
  - Categories numbered from 4 to 15
- **agevehicle**: Integer variable representing the age of the insured vehicle
  - Ages of vehicles range from 0 to 100 years
- **agedriver**: Integer variable representing the age of the usual driver
  - Ages of usual drivers range from 0 to 100 years
- **bonus**: Premium bonus of the policy – numerical variable. It will not be used in a priori ratemaking.
- **brand**: Brand of the insured vehicle. Classification in categorical levels:
  - 1: Renault, Nissan
  - 2: Peugeot, Citroen
  - 3: Volkswagen, Audi, Skoda, Seat
  - 4: Opel, GM
  - 5: Ford
  - 6: Fiat
  - 10: Mercedes, Chrysler
  - 11: BMW, Mini
  - 12: Japanese and Korean
  - 13: Other European
  - 14: Other Brands
- **Fuel**: Vehicle fuel type. Categorical variable.
  - D: Diesel
  - E: Gasoline
- **popdensity**: Continuous variable with the population density of the area of residence of the policyholder. This variable was used to build the variable Zone. It should not enter the tariff model.
- **region**: Region of the zone of residence of the policyholder. Classification in categorical variable. This variable was used to build the variable Zone. It should not enter the tariff model.
- **popdensity** and **region** are used to build the `zone` variable and should not be included in the tariff model.
- **bonus** is a numerical variable representing the premium bonus of the policy but will not be used in a priori ratemaking.



### Claims Data (file claimsdata.txt) | Attributes

- **n**: Unique identifier for the claim record.
- **ncontract**: Number of contracts.
- **coverage**: Type of coverage. We are only interested in 3rd Party Liability Coverage, which is registered as "1RC".
- **cost**: Severity of the claim, measured in terms of cost.

## Additional Information

- The dataset focuses exclusively on 3rd Party Liability Coverage (`coverage` = "1RC").
- Each claim is uniquely identified by the attribute `n`.
- The `ncontract` attribute links the claim data to the corresponding insurance policy contract.
- The `cost` attribute represents the monetary value of the claim, indicating its severity.
