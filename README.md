# getting_cleansing_data

Data Cleaning - Smartphone Activity Recognition

The original dataset is borrowed from the UCI Human Activity Using Smartphones project (http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones). The dataset is for activity recognition (walking, walking upstairs, walking downstairs, sitting, standing, and laying) from smartphone low level sensor data.

The 'run_analysis.R' script contains five function calls that clean up the original dataset in various ways (See deatils in the Functions section below).

File Structure Requirement

To call the functions in the run_analysis.R script, the data Human Activity Recognition Using Smartphone Dataset (the extracted 'HCI HAR Dataset' folder) should be located in the same directory as the 'run_analysis.R' file.

e.g., Within the project folder, the following file structure should be kept:

run_analysis.R
[HCI Har Dataset]
-- activity_labels.txt
-- feactures_info.txt
-- features.txt
-- README.txt
-- [test]
-- [train]
The compressed dataset can be downloaded from: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Function Call

To obtain the submitted tidy data set, users need to follow the following two steps:

source the R file: source("run_analysis.R")
call the AvgMerge function: AvgMerge()
AvgMerge.txt is the tidy dataset that is submitted for the project.
[Caution: Running the function call can take a couple of minutes.]

Included Variables

A total of 68 variables are included in the submitted tidy data set. They are the mean and standard deviation values of the raw accelerometer and gyroscope 3-axial row signals. Only the variables of mean() and std() are included and the weighted average of the frequency components (e.g., meanFreq()) is not included in the final data set. For detailed description regarding variables, see the Variables in the Tidy Data Set section in the codebook.md file.

Functions

The code includes five function calls that clean the original dataset in different ways:

Function Name	Goal/Task	Files Used	Output File	Command
SimpleMerge	Merge the training and the test sets into one data set.

1) Subject ID (subject_test.txt and subject_train.txt) is merged as the first column of the merged data set.

2) Activity type (y_test.txt and y_train.txt) is merged as the second column of the merged data set.

3) Descriptive activity information is copied from the activity_labels.txt file.	1) X_test.txt

2) y_test.txt

3) X_train.txt

4) y_train.txt

5) subject_test.txt 

6) subject_train.txt

7) features.txt	SimpleMerge.txt

SimpleMerge()

MeanStdMerge	Extract only the measurments on the mean and standard deviation (as well as subject id and activity type) for each measurement.

1) At the time of this function call, if SimpleMerge.txt does not exist, this function calls the SimpleMerge() function and creates the SimpleMerge.txt file.

2) If the SimpleMerge.txt file does exist, however, this function reads the file, pattern matches the column names for mean and standard deviation using 'grepl' (as well as 'subjectid' and 'activitytype'), and subset only the matched columns.	1) SimpleMerge.txt	MeanStdMerge.txt
MeanStdMerge()

DesVarMerge	Label the data set with descriptive variable names.

1) At the time of this function call, if MeanStdMerge.txt does not exist, this function calls the MeanStdMerge() function and creates the MeanStdMerge.txt file.

2) If the MeanStdMerge.txt file does exist, however, this function reads the file and replace the variable names (column headings) descriptive variable names.	1) MeanStdMerge.txt	DesVarMerge.txt

DesVarMerge()

DesActMerge	Replace activity numbers with descriptive activity names.

1) Descriptive activity information is copied from the activity_labels.txt file.

2) At the time of this function call, if desVarMerge.txt does not exist, this function calls the desVarMerge() function and creates the desVarMerge.txt file.

3) If the desVarMerge.txt file does exist, however, this function reads the file and replace the values of the activity column from numeric code to descriptive activity types.	1) activity_labels.txt 

2) DesVarMerge.txt	DesActMerge.txt

DesActMerge()

AvgMerge	Create a new tidy data set with the average of each variable for each activity and each subject.

1) At the time of this function call, if desActMerge.txt does not exist, this function calls the desActMerge() function and creates the desActMerge.txt file.

2) If the desActMerge.txt file does exist, however, this function reads the file, loop through each subject and each activity type, and calculate average value of each variable in the dataset (of course, excluding the subject id and activity type column).	1) activity_labels.txt 

2) DesActMerge.txt	AvgMerge.txt

AvgMerge()
