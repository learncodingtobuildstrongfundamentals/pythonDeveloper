# Python Developer
Tasks for a Python developer
task-2# Data Science Test
## Description
This script performs data manipulation and visualization tasks using a sample dataset (`data.csv`). Tasks include loading data, cleaning data, performing basic statistical analysis, adding new columns, and visualizing data.

## Requirements

- Python 3.x
- pandas
- matplotlib
- seaborn

## Installation
Download the script and dataset.
Navigate to the directory containing the script and dataset.
Install the required Python packages using pip:
pip install pandas matplotlib seaborn,pandas.

#Functionality
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

Output:
The script generates the following visualizations:
Bar plot of average salary by department.
Histogram of age distribution.
Scatter plot of age vs. salary.
Mean Salary: 57071.42857142857,
Median Salary: 58000.0,
Salary Std Dev: 6293.638860777612,
Average Salary and Age by Department:
    department   salary   age
0   Engineering  58800.0  30.4   
1   Marketing  52500.0  27.5   
2      Sales  59000.0  37.2   


