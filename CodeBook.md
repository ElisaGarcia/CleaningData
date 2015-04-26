##  Code Book data from Human Activity Recognition Using Smartphones Dataset.

Raw Data
======================================

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

### For each record it is provided:

- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment.

## Result/Tidy data

The result data is a data.frame. The first column of this data.frame specifies the subject, the second the type of activity that performs, and the following columns is the mean of the mean and std of the different variables associated to each type of activity.

### Subject: 
from 1 to 30

### Activities
1. Walking
2. Walking.Upstairs
3. Walking.DownStairs
4. Sitting
5. Standing
6. Laying 

### the variables taken from the row data are just those which represent the mean and the variance:
"tBodyAcc-mean()-X"          
"tBodyAcc-mean()-Y"           "tBodyAcc-mean()-Z"           "tBodyAcc-std()-X"           
 "tBodyAcc-std()-Y"            "tBodyAcc-std()-Z"            "tGravityAcc-mean()-X"       
 "tGravityAcc-mean()-Y"        "tGravityAcc-mean()-Z"        "tGravityAcc-std()-X"        
 "tGravityAcc-std()-Y"         "tGravityAcc-std()-Z"         "tBodyAccJerk-mean()-X"      
 "tBodyAccJerk-mean()-Y"       "tBodyAccJerk-mean()-Z"       "tBodyAccJerk-std()-X"       
 "tBodyAccJerk-std()-Y"        "tBodyAccJerk-std()-Z"        "tBodyGyro-mean()-X"         
 "tBodyGyro-mean()-Y"          "tBodyGyro-mean()-Z"          "tBodyGyro-std()-X"          
 "tBodyGyro-std()-Y"           "tBodyGyro-std()-Z"           "tBodyGyroJerk-mean()-X"     
 "tBodyGyroJerk-mean()-Y"      "tBodyGyroJerk-mean()-Z"      "tBodyGyroJerk-std()-X"      
 "tBodyGyroJerk-std()-Y"       "tBodyGyroJerk-std()-Z"       "tBodyAccMag-mean()"         
 "tBodyAccMag-std()"           "tBodyAccMag-mad()"           "tBodyAccMag-max()"          
  "tBodyAccMag-min()"           "tBodyAccMag-sma()"           "tBodyGyroMag-mean()"        
  "tBodyGyroMag-std()"          "tBodyGyroJerkMag-mean()"     "tBodyGyroJerkMag-std()"     
  "fBodyAcc-mean()-X"           "fBodyAcc-mean()-Y"           "fBodyAcc-mean()-Z"          
  "fBodyAcc-std()-X"            "fBodyAcc-std()-Y"            "fBodyAcc-std()-Z"           
  "fBodyAccJerk-mean()-X"       "fBodyAccJerk-mean()-Y"       "fBodyAccJerk-mean()-Z"      
  "fBodyAccJerk-std()-X"        "fBodyAccJerk-std()-Y"        "fBodyAccJerk-std()-Z"       
  "fBodyGyro-mean()-X"          "fBodyGyro-mean()-Y"          "fBodyGyro-mean()-Z"         
  "fBodyGyro-std()-X"           "fBodyGyro-std()-Y"           "fBodyGyro-std()-Z"          
  "fBodyBodyAccJerkMag-std()"   "fBodyBodyGyroMag-mean()"     "fBodyBodyGyroMag-std()"     
  "fBodyBodyGyroJerkMag-mean()" "fBodyBodyGyroJerkMag-std()" 
  
### In the clean data set the  average of each variable for each activity and each subject is found with the names: 
 "mean.tBodyAcc-mean()-X"           
 "mean.tBodyAcc-mean()-Y"          
 "mean.tBodyAcc-mean()-Z"           
 "mean.tBodyAcc-std()-X"           
 "mean.tBodyAcc-std()-Y"           
 "mean.tBodyAcc-std()-Z"           
 "mean.tGravityAcc-mean()-X"       
 "mean.tGravityAcc-mean()-Y"       
 "mean.tGravityAcc-mean()-Z"       
 "mean.tGravityAcc-std()-X"        
 "mean.tGravityAcc-std()-Y"        
 "mean.tGravityAcc-std()-Z"        
 "mean.tBodyAccJerk-mean()-X"     
 "mean.tBodyAccJerk-mean()-Y"      
 "mean.tBodyAccJerk-mean()-Z"      
 "mean.tBodyAccJerk-std()-X"       
 "mean.tBodyAccJerk-std()-Y"       
 "mean.tBodyAccJerk-std()-Z"       
 "mean.tBodyGyro-mean()-X"          
 "mean.tBodyGyro-mean()-Y"         
 "mean.tBodyGyro-mean()-Z"         
 "mean.tBodyGyro-std()-X"          
"mean.tBodyGyro-std()-Y"          
 "mean.tBodyGyro-std()-Z"          
 "mean.tBodyGyroJerk-mean()-X"      
 "mean.tBodyGyroJerk-mean()-Y"     
 "mean.tBodyGyroJerk-mean()-Z"      
 "mean.tBodyGyroJerk-std()-X"      
 "mean.tBodyGyroJerk-std()-Y"       
 "mean.tBodyGyroJerk-std()-Z"      
 "mean.tBodyAccMag-mean()"          
 "mean.tBodyAccMag-std()"          
 "mean.tBodyAccMag-mad()"           
 "mean.tBodyAccMag-max()"          
 "mean.tBodyAccMag-min()"          
 "mean.tBodyAccMag-sma()"          
 "mean.tBodyGyroMag-mean()"         
 "mean.tBodyGyroMag-std()"         
 "mean.tBodyGyroJerkMag-mean()"    
 "mean.tBodyGyroJerkMag-std()"     
 "mean.fBodyAcc-mean()-X"           
 "mean.fBodyAcc-mean()-Y"          
 "mean.fBodyAcc-mean()-Z"           
 "mean.fBodyAcc-std()-X"           
 "mean.fBodyAcc-std()-Y"            
 "mean.fBodyAcc-std()-Z"           
 "mean.fBodyAccJerk-mean()-X"       
 "mean.fBodyAccJerk-mean()-Y"      
 "mean.fBodyAccJerk-mean()-Z"       
 "mean.fBodyAccJerk-std()-X"       
 "mean.fBodyAccJerk-std()-Y"        
 "mean.fBodyAccJerk-std()-Z"       
 "mean.fBodyGyro-mean()-X"          
 "mean.fBodyGyro-mean()-Y"         
  "mean.fBodyGyro-mean()-Z"          
  "mean.fBodyGyro-std()-X"          
 "mean.fBodyGyro-std()-Y"           
 "mean.fBodyGyro-std()-Z"          
 "mean.fBodyAccMag-mean()"          
 "mean.fBodyAccMag-std()"          
 "mean.fBodyBodyAccJerkMag-mean()" 
 "mean.fBodyBodyAccJerkMag-std()"  
 "mean.fBodyBodyGyroMag-mean()"    
 "mean.fBodyBodyGyroMag-std()"     
 "mean.fBodyBodyGyroJerkMag-mean()" 
 "mean.fBodyBodyGyroJerkMag-std()" 