CourseProj
==========

CourseProject of Coursera's Getting and Cleaning Data course

==================================================================
AIM:

The R program creates takes training and test data sets and merges them together to produce a single data set and certain transforms are performed to obtain a desired tidy data set.

==================================================================
PROCESS:

- The data are read using read.table() function and since the test and trainin data sets are independent observations, rbind() is used to append the data sets. Also, cbind() function is used to combine the variables, subject, activity and 561 feature vector.  

- To ensure readable activity column, factors are used to label activities 1,2,3,4,5,6 as "WALKING","WALKING_UPSTAIRS","WALKING_DOWNSTAIRS","SITTING","STANDING","LAYING" respectively


- Sensible and understandable feature variables are provided and are assigned to colnames of the dataframe

- grepl function is used to extract only those columns which have the string mean in them

- Tidy dataset requires that the mean is to be calculated for each combination of subject and activity. This is done using aggregate() function.

- The tidy data set obtained is ordered by Subject and Activity columns so that all the activities of a subject appear one below the other

- The ordered tidy data set is written to a file using write.table() 



