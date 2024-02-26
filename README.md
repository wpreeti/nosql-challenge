# Module 12 Challenge - NoSQL Databases

Instructions

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

Challenge Instructions

This Challenge is divided into three parts:

Part 1: Database and Jupyter Notebook Set Up
Part 2: Update the Database
Part 3: Exploratory Analysis
Part 1: Database and Jupyter Notebook Set Up

Use NoSQL_setup_starter.ipynb for this section of the challenge.
Import the data provided in the establishments.json file from your Terminal. Name the database uk_food and the collection establishments. Copy the text you used to import your data from your Terminal to a markdown cell in your notebook.
Create an instance of the Mongo Client.
Confirm that you created the database and loaded the data properly:
List the databases you have in MongoDB. Confirm that uk_food is listed.
List the collection(s) in the database to ensure that establishments is there.
Find and display one document in the establishments collection using find_one and display with pprint.
Assign the establishments collection to a variable to prepare the collection for use.
Part 2: Update the Database

Use NoSQL_setup_starter.ipynb for this section of the challenge.
The magazine editors have some requested modifications for the database before you can perform any queries or analysis for them. Make the following changes to the establishments collection:
An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis. Add the following information to the database:
{
 "BusinessName":"Penang Flavours",
 "BusinessType":"Restaurant/Cafe/Canteen",
 "BusinessTypeID":"",
 "AddressLine1":"Penang Flavours",
 "AddressLine2":"146A Plumstead Rd",
 "AddressLine3":"London",
 "AddressLine4":"",
 "PostCode":"SE18 7DY",
 "Phone":"",
 "LocalAuthorityCode":"511",
 "LocalAuthorityName":"Greenwich",
 "LocalAuthorityWebSite":"http://www.royalgreenwich.gov.uk",
 "LocalAuthorityEmailAddress":"health@royalgreenwich.gov.uk",
 "scores":{
     "Hygiene":"",
     "Structural":"",
     "ConfidenceInManagement":""
 },
 "SchemeType":"FHRS",
 "geocode":{
     "longitude":"0.08384000",
     "latitude":"51.49014200"
 },
 "RightToReply":"",
 "Distance":4623.9723280747176,
 "NewRatingPending":True
 }
Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
Update the new restaurant with the BusinessTypeID you found.
