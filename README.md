# Crowdfunding_ETL

This ReadMe serves to:
   1. Certify that this work is our own,
      Lakia White
      Brittney Watts
   3. Specify code source and its location in my 'crowdfunding_ETL' repository,
   4. Clarify the reason for the assignment,

1. 
In this repository, we are implementing our knowledge and skills in the ETL(extract, transform, and load) process to complete deliverable Project 2, "Crowdfunding_ETL".

2. 
The source code is our interpretation of the information we learned with debugging help from forums. Below here
is a breakdown of the locations of each element of our assignment:

    Crowdfunding_ETL
        ETL Project
            Resources
                campaign.csv
                category.csv
                contacts.csv
                ccontacts.xlsx
                crowdfunding.xlsx
                subcategory.csv
            ETL_Mini_Project_LWhite_BWatts.ipynb
         README.md

ETL Challenge:
   Our task was to read the data from the csv files and perform queries on the dataset! For parts 1 and 2, we set up the database to be used in MongoDB and edit the data in preparation for an exploratory analysis. In this analysis, we pull data from the table to analyze and make conlusions on which restaurants in the dataset to eat from. 
   The establishments.json file lists Businesses, their addresses, their websites, and other information. 
   
   My Steps: 

    - First, I had to connect to the SQLite database, reflect the tables into classes, save the references to the classes, and link python to the database all using SQLAlchemy.

    - PART 1: DATABASE AND JUPYTER NOTEBOOK SET UP
        - Using NoSQL_setup_starter.ipynb, I imported the data from the terminal, named a database and its collection. I made sure to copy the text I used for the import statement into the notebook as a markdown cell.
        - Import the libraries, create an instance of MongoClient.
        - Listed the databases, collection, and a document in MongoDB to confirm the creation of the 'uk_food' database, 'establishments' collection, and properly loaded documents.
        - Lastly, I assigned the collection to a variable to use later.

    - PART 2: UPDATE THE DATABASE
        - Add data for a Halal Restaurant to the database.
        - Find the BusinessTypeID and update the new restaurant with the information.
        - Check how many documents contain the Dover Local Authority and remove them. Check the number of documents so we know it's been deleted.
        - Use update_many to convert latitute and longitude to decimal numbers and the RatingValue to integers because they are in the database as strings.
    
    - PART 3: EXPLORATORY ANALYSIS
        - Using NoSQL_analysis_starter.ipynb, this part of the challenge explores the database and answers questiong about the establishments.
        - Display the number of documents in the result and convert the result to a Pandas DataFrame then display the first 10 rows.
        - Find the establishments that have a hygiene score equal to 20, which establishments in London that have a RatingValue greater than or equal to 4, find the top 5 establisments with a RatingValue of 5 (sorted by the lowest hygiene score, newarest to the new restaurant "Penang Flavors"?)
        - Find how many establishments in each Local Authority area have a hygiene score of 0 and sort the results from highest to lowest then print the top ten local authority areas.

      
THANK YOU!!!!!
