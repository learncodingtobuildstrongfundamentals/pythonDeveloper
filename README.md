# Python Developer
Tasks for a Python developer

## Level 1 - Python Developer
Follow instructions in the README.md file in the Level 1 folder.
Make sure to complete both the tasks.
task-1 Create a simple FastAPI service that provides weather data and 
supports basic user authentication with hardcoded values, 
including comprehensive error handling.

This is simple FastAPI application that provides weather data and supports basic user authentication with hardcoded values.
Endpoints
fastapi: The main framework used to create the API.
uvicorn: An ASGI server used to run the FastAPI application.
python-multipart: A package required for handling form data, particularly useful for handling file uploads.
packages:
First install the required packages using pip:
pip install fastapi uvicorn python-multipart,
pip uvicorn main:app --reload
to access the application at http://127.0.0.1:8000
go to http://127.0.0.1:8000/docs.
Details about the login endpoint:
1. /login
Purpose: Allows users to log in and receive a token for authentication.
Method: POST
Request: Requires username and password in the body.
Response: Returns a token if the login is successful.
2./weather/{city}
Purpose: Provides weather data for a specified city.
Method: GET
Request: Requires an authorization token in the header (Authorization: Bearer <token>).
Response: Returns weather data (temperature, humidity, and description) for the specified city.
Note: This endpoint is protected and can only be accessed with a valid token obtained from the /login endpoint.
Hardcoded Data
Weather Data
The weather data for three cities is hardcoded into the application. Each city has the following information:

New York

Temperature: 22°C
Humidity: 60%
Description: Sunny
Los Angeles

Temperature: 25°C
Humidity: 50%
Description: Partly Cloudy
Chicago

Temperature: 18°C
Humidity: 55%
Description: Rainy
User Credentials
The application uses hardcoded user credentials for login:
Username: testuser
Password: testpass

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

