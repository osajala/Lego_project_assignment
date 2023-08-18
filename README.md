# Lego_project_assignment
Lego project is an assignment for the DTSC 580: Data Manipulation, which is part of the requirement for the award of MS in Data Science from Eastern University, Pennsylvania
## Overview

In this assignment, you will load the various tables from the [Rebrickable](https://rebrickable.com/) website and perform analysis on the data.  Rebrickable is a fantastic website that is used to show you which LEGO sets you can build from the sets and parts you already own.  They will even show you which parts you are missing to complete the new set and suggest sets that you could purchase to get those parts.  

## Data

The data has been downloaded directly from their website and includes files for the tables shown in the schema above.  Your first task will be to go through the data and review the schema to understand how the tables all fit together.  There is no data dictionary that I am aware of, but you should be able to understand this data by reviewing the files and schema and visiting their [Download](https://rebrickable.com/downloads/) page and [API](https://rebrickable.com/api/) documentation.  **Note that you must use the files downloaded from Brightspace for this assignment and not download new files from the Rebrickable website.**

## Assignment

In this assignment, you will create a number of functions to complete certain tasks.  This is not needed if you were working on this project on your own, but since we want to see if you can select the data via Pandas/Numpy, we will use those functions in the automatic grading in CodeGrade.  Without this, students could try to look up the answers in the `csv` files instead of wrangling the data with Python/Pandas, which would defeat the purpose of this class.

In addition, we would strongly suggest that you merge data sets as appropriate for the given task.  For example, you might merge the `sets` and `themes` DataFrames to answer one question, and then merge `sets`, `inventories`, `inventory_minifigs`, and `minifigs` to answer another.  This will make your code much easier to write and will be key in working with data across multiple tables.  In fact, I was able to create each function with only one line of code because of the merging of certain data sets.  Also note that you may not use all the tables in this assignment.  This is also an important skill for a Data Scientist to know when to use data and what data is unnecessary.

When complete, save your notebook as `lego.ipynb` and submit to CodeGrade for automatic grading.

## Note

<u>Show Work</u>

Remember that you must show your work.  Students submissions are spot checked manually throughout the term to verify that they are not hard coding the answer from looking only in the file or in CodeGrade's expected output.  If this is seen, the student's answer will be manually marked wrong and their grade will be changed to reflect this. 

For example, if the answer to Q1, the mean of a specific column, is 22:
```
# correct way
Q1 = df['column_name'].mean()

# incorrect way
Q1 = 22 
