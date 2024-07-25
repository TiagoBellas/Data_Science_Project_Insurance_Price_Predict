# Insurance-Price-Predict


Insurance Price Prediction Project

Overview

This is a Academic project which aims to develop a machine learning model that accurately predicts insurance prices based on various customer features. By leveraging a dataset containing information about customers and their insurance claims, we aim to provide a reliable tool for predicting future insurance costs.

Insurance companies need to predict the price of premiums for new customers accurately. By analyzing historical data, we can build a model that helps in estimating these prices.

This project employs various machine learning algorithms to achieve this goal and compares their performance to select the best model using Python and R language.



Dataset
The dataset used in this project includes customer information and also contract claims information describe below:

Automobile Portfolio (file autodata.txt):
 ncontract – Number of contract
 exposition – Risk Exposition of each policy during the year
 zone - Zone of Residence. Classification according to the number of inhabitants for Km2
o A (1 a 50) o D (501 a 2000)
o B (51 a 100) o E (2001 a 10000)
o C (101 a 500) o F (>10000)
 power – Power of the vehicle. Classification in categorical levels.
o Categories numbered from 4 to 15
 agevehicle – Integer variable representing the age of the insured vehicle
o ages of vehicle, registered between 0 and 100 years
 agedriver – Integer variable representing the age of the usual driver
o age of the usual driver, registered between 0 and 100 years
 bonus – premium bonus of the policy – numerical variable. It will not be used in a priori
ratemaking.
 brand – Brand of the insured vehicle. Classification in Categorical levels:
o 1 - Renault, Nissan o 10 - Mercedes, Chrysler
o 2 - Peugeout, Citroen o 11 - BMW, Mini
o 3 - Volkwagen, Audi, Skoda, Seat o 12 - Japonese and Corean
o 4 - Opel, GM o 13 – Other European
o 5 - Ford o 14 – Other Brands
o 6 - Fiat
 Fuel – Vehicle fuel type. Categorical variable.
o D - Diesel
o E - Gasoline
 popdensity – Continuous variable with populational density of the área of residence of the
policyholder. This variable was used to build the variable Zone. Should not enter the tariff
model.
 region – region of the zone of residence of the policyholder. Classification in categorical
variable. This variable was used to build the variable Zone. Should not enter the tariff
model.
