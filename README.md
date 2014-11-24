This folder contain a script for cleaning data project for the "Getting and Cleaning Data" course. Data was uploaded to the project's individual page in the Coursera.

The flow of the sript is as follows:

1. Read and merge X test and train data into a single dataset using rbind.
2. Read features file and set up a second row of this table as a variable names for the earlier merged data.
3. Select variable having "means" and "std" in names from the newly formed dataset
4. Merge the means with stdev
5. Read tables for subject test and train data and merge them
6. Repeat the above step for y labels data
7. Read activity labels data and merge it with y labels data by using key - first column "V1"
8. Leave only labels with acitivy descriptions
9. Column-bind earlier dataset with mean and stdev with the acivity descriptions
10. Column-bind this dataset, dd, with the subject table
11. Rename column names for subjects, which is V1 to "subject" and V2 to "activity
12. Convert data frame into data table using data.table pacckage
13. Aggreagte data by means for a combination of a subject and activity
14. Save the outcome into Dataset.txt file.

=======
