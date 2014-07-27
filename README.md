CourseProj
==========

CourseProject of Coursera's Getting and Cleaning Data course

==================================================================
The R program creates takes training and test data sets and merges them together to produce a single data set   

The data are read using read.table() function and since the test and trainin data sets are independent observations, rbind() is used to append the data sets. Also, cbind() function is used to combine the variables, subject, activity and 561 feature vector.  

