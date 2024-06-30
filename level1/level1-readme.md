**Coding Test 1/2: FastAPI Weather Service**

**Objective Part 1 of 2:**
Create a simple FastAPI service that provides weather data and supports basic user authentication with hardcoded values, including comprehensive error handling.

### Requirements:

1. **FastAPI Service:**
   - Create a FastAPI application.

2. **Hardcoded Weather Data:**
   - Provide hardcoded weather data for a few cities.
   - Each city's weather data should include fields like temperature, humidity, and description (e.g., sunny, rainy).

3. **User Authentication:**
   - Use hardcoded values for user credentials.
   - Implement login functionality using FastAPI's authentication features.

4. **Endpoints:**
   - `/login`: Endpoint for user login, returns a token upon successful authentication.
   - `/weather/{city}`: Protected endpoint that returns weather data for a given city. Requires a valid token to access.

5. **Error Handling:**
   - Implement proper error handling for the following scenarios:
     - Invalid login credentials.
     - Accessing the `/weather/{city}` endpoint without a valid token.
     - Requesting weather data for a city that is not in the hardcoded data.
     - Any other general errors that may occur.

### Hardcoded Data:

**Weather Data:**
```python
weather_data = {
    "New York": {"temperature": 22, "humidity": 60, "description": "Sunny"},
    "Los Angeles": {"temperature": 25, "humidity": 50, "description": "Partly Cloudy"},
    "Chicago": {"temperature": 18, "humidity": 55, "description": "Rainy"},
}
```

**User Credentials:**
```python
users = {
    "testuser": {"username": "testuser", "password": "testpass"}
}
```

### Deliverables:

1. **FastAPI Application:**
   - A FastAPI app that meets the requirements described above.

2. **README File:**
   - Instructions on how to set up and run the application.
   - Examples of how to use the endpoints.

### Instructions:

1. **Setup:**
   - Create a virtual environment and install FastAPI and Uvicorn.
   - Write the FastAPI application with the specified endpoints and functionality.

2. **Endpoints:**
   - Implement the `/login` endpoint to accept a username and password, and return a JWT token if the credentials are correct.
   - Implement the `/weather/{city}` endpoint to return the weather data for the specified city, ensuring that the request is authenticated.

3. **Authentication:**
   - Use JWT tokens for authentication.
   - Ensure that the `/weather/{city}` endpoint is protected and can only be accessed with a valid token.

4. **Error Handling:**
   - Implement proper error handling to manage invalid login credentials, unauthorized access, non-existent cities, and general errors.

### Example:

**Login Request:**
```json
POST /login
{
    "username": "testuser",
    "password": "testpass"
}
```

**Login Response:**
```json
{
    "token": "your_generated_jwt_token"
}
```

**Weather Request:**
```json
GET /weather/New York
Headers: {
    "Authorization": "Bearer your_generated_jwt_token"
}
```

**Weather Response:**
```json
{
    "temperature": 22,
    "humidity": 60,
    "description": "Sunny"
}
```

**Error Handling Examples:**

1. **Invalid Login Credentials:**
   - Should return a 401 status code with a message "Incorrect username or password".

2. **Unauthorized Access:**
   - Should return a 401 status code with a message "Could not validate credentials".

3. **City Not Found:**
   - Should return a 404 status code with a message "City not found".

4. **General Error:**
   - Should return a 500 status code with a message "Internal Server Error" for unexpected issues.

### Submission:

1. Package your FastAPI application code and the README file into a ZIP file named `YourName_FastAPIWeatherTest.zip`.
2. Email the ZIP file to [Your Email Address] with the subject line "FastAPI Developer Test Submission – [Your Name]".
3. Submit your completed test by date mentioned in email.

---

**Coding Test 2/2: Data Science with NumPy and pandas**

**Objective Part 2 of 2:**
Evaluate the candidate's proficiency in using NumPy and pandas for data manipulation and basic data science tasks.

### Requirements:

1. **Data Loading:**
   - Load a dataset from a CSV file into a pandas DataFrame.

2. **Data Cleaning:**
   - Handle missing values.
   - Remove duplicates.

3. **Data Manipulation:**
   - Perform basic statistical analysis.
   - Group and aggregate data.
   - Apply transformations to data.

4. **Data Visualization:**
   - Generate basic plots using matplotlib or seaborn.

5. **Error Handling:**
   - Implement error handling to manage issues like missing files, invalid data, and other potential exceptions.

### Dataset:

Use the following sample dataset for this test. Save it as `data.csv`:

```csv
id,name,age,salary,department
1,John Doe,28,50000,Engineering
2,Jane Smith,34,60000,Marketing
3,Bob Johnson,45,,Sales
4,Alice Williams,29,55000,Engineering
5,Chris Davis,23,48000,Marketing
6,Emma Wilson,38,62000,Sales
7,Olivia Brown,30,60000,Engineering
8,Liam Taylor,31,59000,Engineering
9,Ava Anderson,27,52000,Marketing
10,Isabella Thomas,,58000,Sales
11,Noah Martin,29,52000,Sales
12,Mason Martinez,26,50000,Marketing
13,Ethan Jackson,34,70000,Engineering
14,James White,44,65000,Sales
```

### Tasks:

1. **Data Loading:**
   - Load the `data.csv` file into a pandas DataFrame.

2. **Data Cleaning:**
   - Identify and fill missing values in the `age` and `salary` columns with the median of their respective columns.
   - Remove any duplicate rows based on the `id` column.

3. **Data Manipulation:**
   - Calculate the mean, median, and standard deviation of the `salary` column.
   - Group the data by `department` and calculate the average `salary` and `age` for each department.
   - Add a new column `salary_above_50000` which indicates whether the `salary` is above 50000 (True/False).

4. **Data Visualization:**
   - Create a bar plot showing the average `salary` for each `department`.
   - Create a histogram of the `age` column.
   - Create a scatter plot showing the relationship between `age` and `salary`.

5. **Error Handling:**
   - Implement error handling for:
     - Missing or inaccessible `data.csv` file.
     - Missing or invalid data in the `data.csv` file.
     - Any other potential exceptions that may occur during data processing and visualization.

### Deliverables:

1. **Python Script:**
   - A Python script (`YourName_DataScienceTest.py`) containing:
     - The code for each task.
     - Comments explaining your approach and results.
     - Visualizations with appropriate titles and labels.
     - Error handling for each task.

2. **README File:**
   - A README file with instructions on how to set up and run the script.

### Submission:

1. Package your Python script and README file into a ZIP file named `YourName_DataScienceTest.zip`.
2. Email the ZIP file to [Your Email Address] with the subject line "Data Science Test Submission – [Your Name]".
3. Submit your completed test by Date mentioned in email.
