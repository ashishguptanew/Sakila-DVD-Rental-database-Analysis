# Sakila-DVD-Rental-database-Analysis
Analysis of Sakila DVD Rental database using SQL/PostgreSql

Introduction
In this project, you have queried the Sakila DVD Rental database. The Sakila Database holds information about a company that rents movie DVDs. For this project, we have querying the database to gain an understanding of the customer base, such as what the patterns in movie watching are across different customer groups, how they compare on payment earnings, and how the stores compare in their performance. To assist you in the queries ahead, the schema for the DVD Rental database is used 


Setting up your local environment

What is PostgreSQL?
PostgreSQL is an open-source object-relational database system that is used frequently in industry (and that is running in the background of the SQL queries you have been running in the classroom). At some point, you may find yourself learning how to use this platform and running the application locally on your machine. However, learning to use and manage the PostgreSQL applications is in itself a challenge. If you decide to use the PostgreSQL platform, we strongly advise that you set aside some time for getting familiar with the environment before beginning this project. You will find this step well worth the effort!

Let's set up your local environment

What is PostgreSQL?
PostgreSQL is an object-relational database management system. Object-relational databases use a hybrid approach to databases.

In object databases, information is stored as objects, much like object-oriented programming.
In relational databases, information is stored in tables with relationships between tables defined by primary and foreign keys.
Importantly, PostgreSQL allows the use of advanced functions (such as Window Functions), and even development and use of custom functions written in different programming languages. Here is a link to better understand what is meant by an object-relational database, and how it differs from a relational database.

https://en.wikipedia.org/wiki/Object-relational_database


Ready to proceed with PostgreSQL? Follow along!

Step 1. Downloading PostgreSQL
First, you will need to install PostgreSQL on your local machine. The instructions below provide detailed description of the steps you need to take.

Installing PostgreSQL for Windows:
http://www.postgresqltutorial.com/install-postgresql/

Installing PostgreSQL for Mac OS:
https://www.postgresql.org/download/macosx/

Friendly reminder! Please write down the database superuser (postgres) password as you will need it to create the Sakila database once you have installed the PostgreSQL server.


Step 2. Downloading Sakila database
Once PostgreSQL server is installed, you will need to download the Movie database from this page: PostgreSQL Sample Database

Scroll down and click on the orange "Download DVD Rental Sample Database" button.

This will download a zipped file, and you will need to extract the dvdrental.tar file.


Step 3. Loading database
The next step is to load the DVD Rental database into your PostgreSQL server on your machine. We recommend using the PgAdmin tool. You will find the instructions to do so on the following link: Load PostgreSQL Sample Database.

The instructions are down ⅓ on this page under the header “Load the DVD Rental database using pgAdmin tool” .

The screenshot below shows the blue arrow pointing to the header.

Now follow the instructions all the way through the header titled "Verify the loaded sample database."

Once you have followed the instructions through the end of "Verify the loaded sample database.", you have now loaded the dvdrental sample database into your local PostgreSQL database server.


Step 4. Connecting back to the PostgreSQL server:
Relaunch PgAdmin III and click on the PostgreSQL server within the Object browser. The screenshot below shows the red arrow 
pointing to PostgreSQL server. Click it and enter your superuser (postgres) password.


Step 5. Connecting to the DVD rental database:
Next click on the plus sign next to Databases to access the DVD rental database. The screenshot below shows the red arrow pointing to Databases.


Step 6. Choose the DVD Rental database
Choose the dvdrental database under Databases. The red arrow in the screenshot is pointing towards the dvdrental database.

You should now be linked to the DVD rental database.


Step 7. Running Queries on your dvdrental database
Ready to run some queries?? Click on the SQL icon with a magnifying glass (see the screenshot below with the red square on the icon).

Questions to work upon for analysis
Question 1
We want to find out how the two stores compare in their count of rental orders during every month for all the years we have data for. Write a query that returns the store ID for the store, the year and month and the number of rental orders each store has fulfilled for that month. Your table should include a column for each of the following: year, month, store ID and count of rental orders fulfilled during that month


Question 2
We want to understand more about the movies that families are watching. The following categories are considered family movies: Animation, Children, Classics, Comedy, Family and Music.
Create a query that lists each movie, the film category it is classified in, and the number of times it has been rented out.

Question 3
Now we need to know how the length of rental duration of these family-friendly movies compares to the duration that all movies are rented for. Can you provide a table with the movie titles and divide them into 4 levels (first_quarter, second_quarter, third_quarter, and final_quarter) based on the quartiles (25%, 50%, 75%) of the rental duration for movies across all categories? Make sure to also indicate the category that these family-friendly movies fall into.

Question 4
Finally, provide a table with the family-friendly film category, each of the quartiles, and the corresponding count of movies within each combination of film category for each corresponding rental duration category. The resulting table should have three columns:
-Category
-Rental length category
-Count
