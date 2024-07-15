# Python Developer
Tasks for a Python developer

## Level 1 - Python Developer
Follow instructions in the README.md file in the Level 1 folder.
Make sure to complete both the tasks.
# Data Science Test
#

## Description

This script performs data manipulation and visualization tasks using a sample dataset (`data.csv`). Tasks include loading data, cleaning data, performing basic statistical analysis, adding new columns, and visualizing data.

## Requirements

- Python 3.x
- pandas
- matplotlib
- seaborn

## Installation

1. Download the script and dataset.
2. Navigate to the directory containing the script and dataset.

Install the required Python packages using pip:

```bash
pip install pandas matplotlib seaborn
Dataset
The dataset data.csv contains the following columns:

id: Unique identifier for each record.
name: Name of the employee.
age: Age of the employee.
salary: Salary of the employee.
department: Department of the employee.
Functionality
Data Loading:

Loads the data.csv file into a pandas DataFrame.
Data Cleaning:

Fills missing values in the age and salary columns with the median.
Removes duplicate rows based on the id column.
Data Manipulation:

Calculates and prints the mean, median, and standard deviation of the salary column.
Groups the data by department and calculates the average salary and age for each department.
Adds a new column salary_above_50000 indicating whether the salary is above 50000.
Data Visualization:

Creates a bar plot showing the average salary for each department.
Creates a histogram of the age column.
Creates a scatter plot showing the relationship between age and salary.
Error Handling:

Handles errors for missing or inaccessible data.csv file.
Output
The script generates the following visualizations:

Bar plot of average salary by department.
Histogram of age distribution.
Scatter plot of age vs. salary.
The cleaned dataset is saved as cleaned_data.csv.
