# Credit-Card-Fraud-Detection-
ML Project Credit Card Fraud Detection
MACHINE LEARNING PROJECT 
CREDIT CARD FRAUD DETECTION 

LIBRARIES USED/ IMPORTED
PANDAS:-TO MAKE STRUCTURED DATAFRAME OF DATASETS
NUMPY:-DATASETS CAN BE REFINED AS ARRAY 
SKLEARN 
Work flow for programme: 
Work flow:
 
Step 1:LOADING DATASETS
Dataset downloaded from kaggle.
Step 2: data preprocessing
Data can be processed by using numpy.structured data in 2D Dataframe
Steps for preprocessing :-
1.Uploading datastes and reading using pandas read_csv module
{data=pd.read_csv(“file_path/file_name”)}
2.distribution for ligit and fraud transaction using 
Splitting –
fraud = data[data['Class'] == 1]1 represents fraud/false transaction in datasets
ligit =data[data[‘class]==0]{0 represents true transaction in the datasets.

3.stastical measure of data 
Ligit amount.describe()
Fraud amount.describe()
4.compare the values for both transactions
Data.groupby(‘Class’).mean(){groups data according to their mean}
5.undersamplingbuilding a sample dataset containing similar dataset.
Ligit_sample=ligit.sample(n=134){selects 134 random data from data(creditcard.}
6. to concatante two dataframes
new_data=pd.concat([legit.sample,fraud],axis=0)
{if axis=0,dataframes will be added 1 by 1}
{if axis=1,dataframes wiil added by columns wise}
Step 3:splitting data into features and targets 
{x=new_data.drop(columns =’Class’,axis=1)
{y= new_data.drop[‘Class’]}
Step 4:splitting data into training data and testing data
1.using {Sklearn model_selection-->train_test_split}
2.model traning 
3.model eavluation
Step 5:accuracy prediction
•	1.using metrics-->accuracy_score











