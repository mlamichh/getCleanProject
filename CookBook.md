---
title: "CookBook"
author: "Madan Lamichhane"
date: "November 21, 2015"
---
## Project description
The purpose of the project is to prepare tidy data set obtained from the 
raw data obtained from the experiments carried out with the group of 30 
volunteers.Each person performed six different activities (Walking,
Walking upstairs, Walking donwstairs, Sitting, Standing, and Laying) 
wearing samrtphones and different sensors data have been recorded at the
frequency of 50 Hz. The activity associated with the person has been recorded
manually from video recording.

## Data set Information.
Data has been collected thourgh singals from the accelerometer and gyroscope in the Samsung
galaxy S II. These singals are pre-processed by applying noise filters and sampled in fixed-width
sliding windows of 2.56 sec and 50 % overlap.

## Signals

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

- tBodyAcc-XYZ
- tGravityAcc-XYZ
- tBodyAccJerk-XYZ
- tBodyGyro-XYZ
- tBodyGyroJerk-XYZ
- tBodyAccMag
- tGravityAccMag
- tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag 

## Variables

The set of variables estimated for above signals are:

- mean(): Mean value
- std(): Standard deviation
- mad(): Median absolute deviation 
- max(): Largest value in array
- min(): Smallest value in array
- sma(): Signal magnitude area
- energy(): Energy measure. Sum of the squares divided by the number of values. 
- iqr(): Interquartile range 
- entropy(): Signal entropy
- arCoeff(): Autorregresion coefficients with Burg order equal to 4
- correlation(): correlation coefficient between two signals
- maxInds(): index of the frequency component with largest magnitude
- meanFreq(): Weighted average of the frequency components to obtain a mean frequency
- skewness(): skewness of the frequency domain signal 
- kurtosis(): kurtosis of the frequency domain signal 
- bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.
- angle(): Angle between to vectors.

Angles variables:

- gravityMean
- tBodyAccMean
- tBodyAccJerkMean
- tBodyGyroMean
- tBodyGyroJerkMean

## Data transformation
The data transformation from raw data to tidy is done by using "run_analysis.R" script.

- Mearge training and test data set: Both test and training data set are merged to get
single data set.

- Extract mean and standard deviation: Extracts measurements only associated with mean
and standarded deviation for each measurement.

- Provide descriptive varaible names: It is important to provide the column names which
clearly represents the variable names hence this step rewrite variable names in clear form
with out brackets, dashes and commas.

- Create tidy data set: In the final data set activity level are clearly labeled, each 
individual are associated with unique identifier, and there are 87 signal variable 
associated with mean and stadard deviation of the different singals.
