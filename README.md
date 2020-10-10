# TravelApp
Project Based Learning:
TravelFar App
Project Overview:
You have been hired to implement the backend functionality for a travel app. The task is to return the correct data to a user’s search. 
Files you will need:
    • index.html contains the front end design of the website.
    • index.js contains the back end functionality.
    • Database,json contains the local database  
# Task 1:
The first task to complete is when a user searches you need to make sure that their input is in the same format as the data in the database. Have a look at the database,json file to see how the names look (Hint: capitalisation). Then you need to make sure that the user’s input is in the same format.
# Task 2:
Now you need to find the correct data from the database. This will occur in the function readFile() which is called when the user searches for a term. Here you will need to search through each country name to check if it is the same data as the user’s search and then show the information about this country to the user. 
# Task 3:
This task is error handling. If you cannot find the information in the database that you need then to alert the user why it has not worked. 
# Task 4: Tricky!
There is an algorithm called the levenshtein algorithm. This takes an input of two strings and checks how similar they are by the number of different letters. For instance the string “Albania” and “Albanie” would return 1 as there is 1 letter difference.
The algorithm has been provided for you at the bottom of index.js and can be called like this:

`levenshtein("Albanie", "Albania");`

This is a really useful function when a user misspells their search term input. See if you can provide the user with a short list of countries that they could have meant (in the case that there is no match in the database for what they have searched).
The smalldatabase.json file has been provided with only countries beginning with A inside. This means you can test you code quickly and easily to see if it works. Try see if you can show 3 countries with small levenshtein distances when a user misspells a country,

Hint 1 – this will need to happen when there is no match in the database

Hint 2 – after you find there is no match then you will need to go through the database again (this time the smalldatabase.json file) and check the levenshtein distance. When doing this you will need to be storing this result somewhere so that you can show it to the user! (something like an array would work).
