# Identification for Potential Insurance Customers
This is the capstone project for the course - Advanced Data Science with IBM Specialization.<br>
This project was completed on IBM cloud with Spark, SparkSQL and Python.<br>
A Code pre-view is available with the file DS Capstone_Insurance Purchasing Analysis.pdf.<br>

## Project Overview
This data set used in the CoIL 2000 Challenge contains information on customers of an insurance company. <br>
The data consists of 86 variables and includes product usage data and socio-demographic data derived from zip area codes. <br>
The data was collected to answer the question: how to identify the potential customers?<br>

## Data Source
The data file contains the following fields:<br>

ORIGIN: train or test, as described above<br>
MOSTYPE: Customer Subtype; see L0<br>
MAANTHUI: Number of houses 1 - 10<br>
MGEMOMV: Avg size household 1 - 6<br>
MGEMLEEF: Avg age; see L1<br>
MOSHOOFD: Customer main type; see L2<br>
** Percentages in each group, per postal code (see L3)<br>
MGODRK: Roman catholic<br>
MGODPR: Protestant <br>
MGODOV: Other religion<br>
MGODGE: No religion<br>
MRELGE: Married<br>
MRELSA: Living together<br>
MRELOV: Other relation
MFALLEEN: Singles<br>
MFGEKIND: Household without children<br>
MFWEKIND: Household with children<br>
MOPLHOOG: High level education<br>
MOPLMIDD: Medium level education<br>
MOPLLAAG: Lower level education<br>
MBERHOOG: High status<br>
MBERZELF: Entrepreneur<br>
MBERBOER: Farmer<br>
MBERMIDD: Middle management<br>
MBERARBG: Skilled labourers<br>
MBERARBO: Unskilled labourers<br>
MSKA: Social class A<br>
MSKB1: Social class B1<br>
MSKB2: Social class B2<br>
MSKC: Social class C<br>
MSKD: Social class D<br>
MHHUUR: Rented house<br>
MHKOOP: Home owners<br>
MAUT1: 1 car<br>
MAUT2: 2 cars<br>
MAUT0: No car<br>
MZFONDS: National Health Service<br>
MZPART: Private health insurance<br>
MINKM30: Income < 30.000<br>
MINK3045: Income 30-45.000<br>
MINK4575: Income 45-75.000<br>
MINK7512: Income 75-122.000<br>
MINK123M: Income >123.000<br>
MINKGEM: Average income<br>
MKOOPKLA: Purchasing power class<br>

** Total number of variable in postal code (see L4):<br>
PWAPART: Contribution private third party insurance<br>
PWABEDR: Contribution third party insurance (firms) <br>
PWALAND: Contribution third party insurane (agriculture)<br>
PPERSAUT: Contribution car policies<br>
PBESAUT: Contribution delivery van policies<br>
PMOTSCO: Contribution motorcycle/scooter policies<br>
PVRAAUT: Contribution lorry policies<br>
PAANHANG: Contribution trailer policies<br>
PTRACTOR: Contribution tractor policies<br>
PWERKT: Contribution agricultural machines policies<br>
PBROM: Contribution moped policies<br>
PLEVEN: Contribution life insurances<br>
PPERSONG: Contribution private accident insurance policies<br>
PGEZONG: Contribution family accidents insurance policies<br>
PWAOREG: Contribution disability insurance policies<br>
PBRAND: Contribution fire policies<br>
PZEILPL: Contribution surfboard policies<br>
PPLEZIER: Contribution boat policies<br>
PFIETS: Contribution bicycle policies<br>
PINBOED: Contribution property insurance policies<br>
PBYSTAND: Contribution social security insurance policies<br>
AWAPART: Number of private third party insurance 1 - 12<br>
AWABEDR: Number of third party insurance (firms) <br>
AWALAND: Number of third party insurance (agriculture)<br>
APERSAUT: Number of car policies<br>
ABESAUT: Number of delivery van policies<br>
AMOTSCO: Number of motorcycle/scooter policies<br>
AVRAAUT: Number of lorry policies<br>
AAANHANG: Number of trailer policies<br>
ATRACTOR: Number of tractor policies<br>
AWERKT: Number of agricultural machines policies<br>
ABROM: Number of moped policies<br>
ALEVEN: Number of life insurances<br>
APERSONG: Number of private accident insurance policies<br>
AGEZONG: Number of family accidents insurance policies<br>
AWAOREG: Number of disability insurance policies<br>
ABRAND: Number of fire policies<br>
AZEILPL: Number of surfboard policies<br>
APLEZIER: Number of boat policies<br>
AFIETS: Number of bicycle policies<br>
AINBOED: Number of property insurance policies<br>
ABYSTAND: Number of social security insurance policies<br>
CARAVAN: Number of mobile home policies 0 - 1<br>

## Correlations and Visualizations<br>

## Feature Engineering<br>
Categorical variables: The target mean encoding method was used since the categorical variable MOSTYPE has 41 types.<br>
Numerical variables: Processed with the Standard Scaler<br>

## Model Selection:<br>
LogisticRegressionClassifier<br>
LinearSVC<br>
NaiveBayesClassifier<br>
RandomForestClassifier<br>
GBTClassifier<br>
FMClassifierClassifier<br>

## Solutions for Imbalanced Data:<br>
Oversampling with SMOTE<br>
Hyper-parameter adjustment (e.g.changing threshold)<br>

## Model Tuning: <br>


## Feature Importance:<br>

## Ideas for Further Improvement:<br>
Use a combined re-smapling method - SMOTE & TomekLinks<br>
Use algorithms with the base estimator (e.g.Easy Ensemble Classifier, RUS Boost Classifier)<br>
Train the model with different feature selection methods (e.g. variance threshold filter, feature selection based on the feature importance in LR/RF model)<br>
Tune the model in a more refined way (e.g use the range() function instead of a given list)
