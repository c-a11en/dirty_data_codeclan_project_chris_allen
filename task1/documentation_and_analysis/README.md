Task 1 - Decathlon
================

# Overview

This project is designed to clean and analyse decathlon results data
which includes scores / times for each athlete and the total score for
that competition.

The project is structured such that the raw data is processed via a data
cleaning script before being analysed to answer a number of set of
questions within an analysis file.

# Packages

The following packages have been used in this project:  
- tidyverse: Reading in raw data, data wrangling functions and use of
pipe (%\>%) operator  
- here: Relative file references for reproducibility from other users  
- janitor: Cleaning column names of meteorite data set

# Data Cleaning

The raw data set is processed via a data cleaning script which prepares
the data for analysis.

The script (“clean_data.R”) reads in the raw data, cleans column names
using the janitor package, converts row names to column and formats
athlete names etc.

The script outputs the cleaned data set into the clean_data folder,
ready for analysis.

# Data Analysis

The cleaned data is read into the analysis Rmd file and analysis is
undertaken, using mostly dplyr functions, to answer the following
questions:

1.  Who had the longest long jump seen in the data?  
2.  What was the average 100m time in each competition?  
3.  Who had the highest total points across both competitions?  
4.  What was the shot-put scores for the top three competitors in each
    competition?  
5.  What was the average points for competitors who ran the 400m in less
    than 50 seconds vs. those than ran 400m in more than 50 seconds?

The outputs of these questions are located in the analysis file
(“data_analysis.Rmd”) along with commentary on any assumptions made to
arrive at the answer.
