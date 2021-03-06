# Zipcode Wilmington Python Data Lab

### Goals

* Learn how to connect to a database in python
* Effectively work with multiple data sources
* Generate a report that is human readable

### Instructions

Two companies are perorming a merger. These two comapnies are Pro-Marketing and MarketingOne.

Both of these companies keep a database full of leads and they want you to combine the two databases into a csv file for marketers to review. Once they review and approve it, you will have to import that data to a new database.

Write a python script that will connect to both databases, pull in the data and export it to a csv. 

After its exported to CSV write a SQL script called `schema.sql` that creates the schema and tables needed for the data you export. Next, write a python script that can read your csv file and run insert statements against your own database.

You must use the csv module along with the mysqlclient and psycopg2 modules. For your benefit I've included the requirements.txt file. You may install everything you need by running `pip install -r requirements.txt` in the base of this project. 

### Turning In

A project should be turned in with at least 4 things.

1. A file called `export.py` that exports the data from the two companies
2. A file called `leads.csv` that should have been generated by export.py
3. A file called `schema.sql` that contains the sql script to create a new database schema/tables for the exported data
4. A file called `import.py` that imports the data from the generated `leads.csv` file

*DO NOT PULL REQUEST SOMETHING WITH THE DATABASE CREDENTIALS IN THE SCRIPT. CREDENTIALS SHOULD BE IN A SEPARATE FILE FROM YOUR MAIN SCRIPT AND THAT FILE SHOULD BE IGNORED IN YOUR GITIGNORE FILE*
