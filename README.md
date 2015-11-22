---
title: "README"
author: "Madan Lamichhane"
date: "November 22, 2015"
---

## Project
The purpose of the project is to generate tidy data set from the given training 
and test data set from the experiment carried out to identify the activities performed
by 30 volunteers. The data has been collected using the signals from the accelerometer
gyroscope present in the smartphones at the frequency of the 30 Hz and activities
are monitored manually using video recording.

##  Files in the repository
- CodeBook.md: Provides information about the raw and tidy data set.Including varaibles
and signal obtained from the samrtphones sensors. 
- README.md: Describe about the project and files present in the repository.
-run_analysis.R: Script to convert raw data into tidy data
-tidyData.txt: Final tidy data for further processing.

## Process to create tidy data set.

1. [download file using the link](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)
2. Unzip folder and save.
3. Open r-studio and set working directory at the saved folder.
4. Run "run_analysis.R" script.
5. The tidy data has been produced as "tidyData.txt" in the folder.




