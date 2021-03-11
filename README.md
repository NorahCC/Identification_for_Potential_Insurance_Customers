# Identification for Potential Insurance Customers
This is the capstone project for the course - Advanced Data Science with IBM Specialization.
This project was completed on IBM cloud with Spark, SparkSQL and Python.
Code pre-view is available with the file DS Capstone_Insurance Purchasing Analysis.pdf.

## Project Overview:
This data set used in the CoIL 2000 Challenge contains information on customers of an insurance company. 
The data consists of 86 variables and includes product usage data and socio-demographic data derived from zip area codes. 
The data was collected to answer the question: how to identify the potential customers?

## Data Source:
The data file contains the following fields:

ORIGIN: train or test, as described above
MOSTYPE: Customer Subtype; see L0
MAANTHUI: Number of houses 1 - 10
MGEMOMV: Avg size household 1 - 6
MGEMLEEF: Avg age; see L1
MOSHOOFD: Customer main type; see L2
** Percentages in each group, per postal code (see L3)
MGODRK: Roman catholic
MGODPR: Protestant …
MGODOV: Other religion
MGODGE: No religion
MRELGE: Married
MRELSA: Living together
MRELOV: Other relation
MFALLEEN: Singles
MFGEKIND: Household without children
MFWEKIND: Household with children
MOPLHOOG: High level education
MOPLMIDD: Medium level education
MOPLLAAG: Lower level education
MBERHOOG: High status
MBERZELF: Entrepreneur
MBERBOER: Farmer
MBERMIDD: Middle management
MBERARBG: Skilled labourers
MBERARBO: Unskilled labourers
MSKA: Social class A
MSKB1: Social class B1
MSKB2: Social class B2
MSKC: Social class C
MSKD: Social class D
MHHUUR: Rented house
MHKOOP: Home owners
MAUT1: 1 car
MAUT2: 2 cars
MAUT0: No car
MZFONDS: National Health Service
MZPART: Private health insurance
MINKM30: Income < 30.000
MINK3045: Income 30-45.000
MINK4575: Income 45-75.000
MINK7512: Income 75-122.000
MINK123M: Income >123.000
MINKGEM: Average income
MKOOPKLA: Purchasing power class

** Total number of variable in postal code (see L4):
PWAPART: Contribution private third party insurance
PWABEDR: Contribution third party insurance (firms) …
PWALAND: Contribution third party insurane (agriculture)
PPERSAUT: Contribution car policies
PBESAUT: Contribution delivery van policies
PMOTSCO: Contribution motorcycle/scooter policies
PVRAAUT: Contribution lorry policies
PAANHANG: Contribution trailer policies
PTRACTOR: Contribution tractor policies
PWERKT: Contribution agricultural machines policies
PBROM: Contribution moped policies
PLEVEN: Contribution life insurances
PPERSONG: Contribution private accident insurance policies
PGEZONG: Contribution family accidents insurance policies
PWAOREG: Contribution disability insurance policies
PBRAND: Contribution fire policies
PZEILPL: Contribution surfboard policies
PPLEZIER: Contribution boat policies
PFIETS: Contribution bicycle policies
PINBOED: Contribution property insurance policies
PBYSTAND: Contribution social security insurance policies
AWAPART: Number of private third party insurance 1 - 12
AWABEDR: Number of third party insurance (firms) …
AWALAND: Number of third party insurance (agriculture)
APERSAUT: Number of car policies
ABESAUT: Number of delivery van policies
AMOTSCO: Number of motorcycle/scooter policies
AVRAAUT: Number of lorry policies
AAANHANG: Number of trailer policies
ATRACTOR: Number of tractor policies
AWERKT: Number of agricultural machines policies
ABROM: Number of moped policies
ALEVEN: Number of life insurances
APERSONG: Number of private accident insurance policies
AGEZONG: Number of family accidents insurance policies
AWAOREG: Number of disability insurance policies
ABRAND: Number of fire policies
AZEILPL: Number of surfboard policies
APLEZIER: Number of boat policies
AFIETS: Number of bicycle policies
AINBOED: Number of property insurance policies
ABYSTAND: Number of social security insurance policies
CARAVAN: Number of mobile home policies 0 - 1

## Correlations and visualizations:

## Feature Engineering
Categorical variables: The target mean encoding method was used since the categorical variable MOSTYPE has 41 types.
Numerical variables: Processed with the Standard Scaler

## Model Selection:
LogisticRegressionClassifier
LinearSVC
NaiveBayesClassifier
RandomForestClassifier
GBTClassifier
FMClassifierClassifier

## Solutions for imbalanced data:
Oversampling with SMOTE
Hyper-parameter adjustment (e.g.changing threshold)

## Model Tuning: 


## Feature Importance:

## Ideas for Further Improvement:
