# Data Cleaner

Current version: 1.0

This tool was created for the task of cleaning data for data analysis. The goal of the final version is to handle all processes of data wrangling such as imputing, recommending machine learning technique, cleaning data, visualizing data.

The initial development of this tool has focused on
the following procedure:
1) Load dataset from csv
2) Change column names according to how the user designates them
3) Collect unique values (non-numerical) within each column for user to determine if values should be normalized or scaled
4) Change all non-numerical values in column with user designated scale
5) Display a renaming key for non-numerical original value to new value
6) Display the dataset prepped for data analysis

As this is only an initial tool, there are plenty of implementations that are being developed. These include:
1) Initially, imputing data by deletion of null-containing rows, for initial analysis
2) A menu interface for repeating functions such as renaming column names
3) Exporting resulting data tables and old:new dictionary for analysis outside of program
4) Summarizing data by mean, mode, std dev, null count, etc.
5) Recommend machine learning technique for classification based on accuracy in initial (impute by delete) cross validation

Down the road implementations are:
1) Using "whole" data points in order to recommend best classifier for imputing null values
2) Determine importance (correlation) to target value by machine learning of binary (1: has data, 0: null data) input
3) Allowing user to select method of imputing (deletion, mode, mean, median, prediction)
4) Visualize locations of null values to help user make quick imputing decisions
5) Visualize data by matplotlib boxplots, histograms, etc.
