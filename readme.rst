###################
Import CSV File Data into MySQL Database using PHP (CodeIgniter)
###################

A CSV (comma-separated values) file stores the tabular data in plain text format. Using CSV file you can store all the data and import the CSV file data into the database at once using PHP and MySQL. Import CSV into MySQL helps to save the user time and avoid repetitive work. In this tutorial, we will show you how to upload and import CSV file data into MySQL database using PHP.

Here we’ll build an example script to import members data into the database. According to this script functionality, the user would be able to upload a CSV file of members details and members data would be inserted into the MySQL database using PHP.

*******************
Step 1: Create Database Table
*******************

You should create a table (member) in the database to store the member’s data. The following SQL creates a member table with some basic fields.

**************************
Step 2: Connect to the Database
**************************

Though we use CodeIgniter 3.1.2, we need to config our database configuration in application->config->database.php file.

*******************
Step 3: Create a view page
*******************

To upload the csv file, we need to create a view page.

************
Step 4: Import CSV Data to Database
************

The following works are processed in this file.

Validates the uploaded file whether it is a valid .csv file.
The is_uploaded_file() function is checks whether the CSV file is uploaded via HTTP POST.
The fopen() function opens the CSV file in read-only mode.
The fgetcsv() function is used to parse the member’s data from the open CSV file. This function is called in the while loop to parse data from CSV file.
Members data are inserted into the database using PHP and MySQL.
At last, the user is redirected to the main page with importing status message.

*******
Conclusion
*******

We hope this script will help you to implement the import feature in your web project easily. Here we’ve discussed the CSV import to MySQL, you can add more fields or restrictions on data import based on your requirement.
