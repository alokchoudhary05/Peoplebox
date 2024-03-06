# **Employee Data Transformation Documentation**


* This script performs data transformation on employee records to extend each employee's data to 15 rows. Below is a concise overview of the methodology and assumptions used:

## **Methodology:**

1. Loading Input Data:
* The script loads input data from a CSV file named input.csv located in Google Drive.

2. **Handling Null Values:**
* Null values in the dataset are handled using forward fill (ffill) and backward fill (bfill) methods to propagate non-null values.

3. **Data Transformation:**
* For each employee record, the script extends the data to 15 rows.
* It calculates tenure in the organization in months and years based on the 'Date of Joining' and 'Date of Exit'.
* The script alternates between two compensation values (20000 and 10000) for each row.
* End dates are set to '2100-01-01' for the first row and '2023-12-30' for subsequent rows.

4. **Saving Output:**
* The resulting extended dataset is saved to a CSV file named 'output.csv.'

## **Assumptions:**

1. **Tenure Calculation:**
* Tenure in the organization is calculated in months and rounded to the nearest month. If the tenure is less than 12 months, it is displayed as '1 year'.

2. **Compensation Alternation:**
* Compensation values alternate between 20000 and 10000 for each row, starting with the initial compensation value.

3. **End Date Assignment:**
* The end date for the first row is set to a far-future date ('2100-01-01'), while subsequent rows have an end date of '2023-12-30'.


## Thank-You
LinkedIn Profile: Alok Choudhary 
[![LinkedIn](LinkedIn-Connect-blue)](https://linkedin.com/in/alok-choudhary9341776554)
