# Wafer-Fault-Detection
Whether wafer should replaced are not

## Data Description
  - The client will send data in multiple sets of files in batches at a given location. Data will contain Wafer names and 590 columns of different sensor values for each wafer.  The last column will have the "Good/Bad" value for each wafer.
  - "Good/Bad" column will have two unique values +1 and -1.  

## Description of folders in the project
**Schema_training.json**
  - Which contains all the relevant information about the training files such as:
      - Name of the files
      - Length of Date value in FileName
      - Length of Time value in FileName
      - Number of Columns
      - Name of the Columns
      - Datatype.

**Schema_prediction.json**

  - Which contains all the relevant information about the training files such as:
      - Name of the files
      - Length of Date value in FileName
      - Length of Time value in FileName
      - Number of Columns
      - Name of the Columns
      - Datatype.
      
**DataTransform_training and DataTransformation_prediction**
>This file contains a class which is used for transforming the Good Raw Training Data before loading it in Database!!.

**Training_Batch_files and Prediction_Batch_files**
> All csv files from the client required for this project.

**Training_Raw_Data_validation and Prediction_Raw_Data_Validation**
>This class shall be used for handling all the validation done on the Raw Prediction Data!!.
>Data Validation is done on Name Validation, Number of Columns, The datatype of columns, Null values in columns 

**TrainingArchivedBadData and PredictionArchivedBadData**
>After validating data bad data will move to these folders.

**DatatypeValidation_Insertion_Training and Datatypevalidation_Insertion_prediction**
>Handling all the SQL operations like database connection, Table creation, Inserting data into database.

**Training Database and Prediction Database**
>It contains .db(database) file

**Training_FilefromDB and Prediction_FilefromDB**
>It contains csv file which is obtained from database

**Data Ingestion**
>To load the data from csv file

**Data Preprocessing**
>Cleaning the data before Training

**Models**
>It contain files that, types of models used for training

**File Operations**
>To save the model after training and load the saved model for prediction.

**Best_model_finder**
>To find the model with best accuracy and AUC score.

**Trainingmodel.py**
>Model Training

**application_logging, Training_logs and prediction_logs**
>Contains log files

**Templates**
>Files used for front end application

**main.py**
>Flask app file starting point of the project

**Procfile**
>Required for deploying the project

**requirements.txt**
>List of libraries required to run this project and to install all the libraries use the below command

`pip install -r requirements.txt`

**runtime.txt**
>It shows which python version is used for to run this project

**predictfromModel.py**
>After training the data, this file is used to predict all prediction_batch files which are inserted in database and loaded into csv file.

**predictionOutputfile**
>Predicted file after doing prediction.


#User Interface
<img src = "file:///E:/WaferFaultDetection_new1/templates/index.html">























