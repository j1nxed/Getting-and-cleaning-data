In the run_analysis.R script, functions were created for each step.

Function r_Data : This function takes two variables, the suffix for the filename, folder name in which the file exists. Since the data exists in two folders with file names as subject_train, X_train, y_train. The y_data file contains Activity_ID. The X_data file contains data for MeasureID and MeasureName. The subject_data file contains SubjectID. This function reads the three files from a folder and creates data.frame in R environment with appropriate column names. The grep function is used to match only those columns which has MeasureName for mean and standard deviation.

Function read_test_data : This function is used to read the test data into the R environment

Function read_train_data : This function is used to read the train data into the R environment

Function mergeDataset : This function combines the two dataset read in the above functions, by rows.Further, proper name is given to the columns and dataset is returned.

Function activityLabels: This function takes a dataset as argument and reads the activity labels from text files and merges it with the dataset.

Function merge_label_data : This function runs the activityLabels function to get a activity labelled dataset.

Function tidyData: This function creates a tidy data set with average of each variable for each activity and each subject.

Function tidy_datafile: A new tidy independent dataset is generated and saved a text file to be submitted.
