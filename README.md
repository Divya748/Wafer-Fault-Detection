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
> All csv files from the client 



























