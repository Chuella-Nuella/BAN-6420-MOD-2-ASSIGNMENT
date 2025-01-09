Overview
This project is developed as part of the BAN6420 - Programming in Python and R course assignment. The focus is on importing, processing, and exporting employee salary data using Python and R, with robust error-handling mechanisms. Below are the tasks and functionalities implemented in the project.
Tasks and Functionalities
Task 0: Import Salary Data
The salary dataset (Total.csv) is imported into the Jupyter Notebook using Python's pandas library.
Error handling ensures that any issues during file loading (e.g., file not found, incorrect format) are captured and reported.
Task 1: Retrieve Employee Details
A Python function salary_function accepts an employee's name as input and retrieves their details from the dataset.
Returns a filtered pandas DataFrame containing the employee's information.
Task 2: Data Processing with Dictionary
A dictionary is constructed from the retrieved employee data. Key details such as JobTitle, BasePay, OvertimePay, TotalPay, and Year are processed for further use.
Task 4: Error Handling
All major operations are wrapped in try-except blocks to ensure exceptions are handled gracefully. Errors are logged with detailed messages.
Task 5: Export and Zip Employee Data
The processed employee details are exported to a CSV file (Employee Profile.csv).
The CSV file is then zipped into a folder named Employee Profile.zip.
The unzipped CSV is deleted after zipping to maintain a clean working directory.
Task 6: Process Zip File in R
The zipped folder (Employee Profile.zip) is unzipped using R.
The extracted CSV file is loaded into R for display and further processing using read.csv and View.
File Structure
The following files and directories are used in the project:
Total.csv: Dataset containing salary data.
Employee Profile.zip: Zipped folder containing the exported employee CSV.
Employee Profile.csv: CSV file containing processed employee data (created and deleted within the Python script).
Prerequisites
Python Requirements:
Python 3.6 or higher
Libraries: pandas, zipfile, os
R Requirements:
R 4.0 or higher
Library: utils
Running the Project
In Python:
1. Ensure Total.csv is in the same directory as the script.
2. Run the Python script:
python script.py
3. Follow the prompts to enter an employee's name.
4. The zipped folder (Employee Profile.zip) containing employee details will be created.
In R:
1. Place the zipped folder (Employee Profile.zip) in your working directory.
2. Run the R script:
source("script.R")
3. The script unzips the folder and displays the employee data.

Error Handling
Python: Logs errors (e.g., missing file, incorrect input) as JSON messages.
R: Captures errors using tryCatch and displays them in a user-friendly format.
