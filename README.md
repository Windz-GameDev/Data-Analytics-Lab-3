# Data-Analytics-Lab-3

Intro:

This is a lab I completed for for my CAP4784 Introduction to Data Analytics class at UNF.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Lab Instructions:

[Data Collection.pdf](https://github.com/Windz-GameDev/Data-Analytics-Lab-3/files/10854184/Data.Collection.pdf)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Description:

In this lab, we created a simple SQLite db for a business, queried an API, and found matching headlines based off certain keywords from the Google News site.
There are two Python scripts in this repository.
  The first script is for creating the SQLlite DB, inserting data, selecting data, and updating it. (Questions 1-8)
  The second script contains a function to query an API and that prints information about the server response, while also containing an example of how 
  to use the query function. It also contains a function for finding headlines by keywords, which contains also contains an example of how to use the function
  within the script.
  
----------------------------------------------------------------------------------------------------------------------------------------------------------------------- 

Important Note:

The script for questions 1-8 may requirement administrator privileges to successfully write to the DB, assuming it has already been created.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Testing:

  Both scripts were developed and run through PyCham using the Python 3.1.1 interpreter.
  As noted above, the script for questions (1-8) will fail to run correctly due to the lack of write permissions to your database 
  if it already exists, and PyCharm is not run as administrator. Drops statement were added to beginning of this script as well to ensure 
  there are no conflicts with the insert statements and duplicate unique ids. The script for questions (9-10) as of 2/28/2023 works without issues
  regarldess of whether it is run as administrator.
  
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Input:

  The scripts currently do not accept any input from the console when run, and the input to the functions are hardcoded in their respective script files.
  
----------------------------------------------------------------------------------------------------------------------------------------------------------------------- 

Output:

  The script for Questions (1-8) outputs a DB to an external SQLite3 db file, and displays the result of four select statements to the console. 
  
  The output of the second script Questions (9-10) also displays to the console.
  
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
Resources Used:

https://www.datamuse.com/api/
-API Used for the test query. Program currently find words that rhyme with forgetful. The DataMuse API does not require an API key. It can be used freely without any authentication. 

https://pypi.org/project/beautifulsoup4/
-Python library used for parsing the html content from the Google News page, and finding the h4 headers.

https://pypi.org/project/requests/
-Used to make a get request to both the api resource, and the google news page to retrieve information. 

https://www.jetbrains.com/pycharm/
-PyCharm was the primary development IDE for this lab.

https://colab.research.google.com/
-Google Collab was a secondary development enviroment for this lab, used for additional development and testing of the script for the questions (9-10).

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
