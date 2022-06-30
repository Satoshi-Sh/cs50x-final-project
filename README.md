# FIND IT
#### Video Demo:  https://www.youtube.com/watch?v=OmVTkURR3UY

#### Description:

Findit lets user explore in movie data in an interactive way.

#### Background

I chose this project because I enjoyed building the finance app through the course and wanted to make an application interacting the database to get used to SQL more. At first, I was planning to use Youtube API to monitor my watching history but the API does't retrieve watching history anymore so decided to do movie search app with the database provided in the SQL course.

#### Website Features

Findit lets user search a director from the movie.db (~2021) we used in the SQL course. In main page, they can search movies by director name. It has autocompletion according to what user types. Once user searched a director, the page shows table of the director works with release year, rating, yearly average score. It also shows an face icon based on the overall rating of the director such as smiling, expression face, and so on. It gives star for each title if the title has much better score than year average. At the bottom, the graph will be displayed. It plots the review of the director and the yearly average of the IMDb score.

The website has two more pages to give user to search by title and actor. Most people don't remember the name of the director. Movie titles come up first and then actor names usually. In the page of find director by title page, user can type in input as the main page, but this time autocompletion shows movie titles and the director name. User can click on suggestions. Once the user clicked one of the suggestion, the director name will be posted to the main page and user can see the main content of this page. In the page of find director by actor,
user can type the actor name, suggestion will be shown once user type any characters. Once user click one of them, the page shows the titles that the actor played with the director name and the released year. User can click the director name, which lead the user to main page showing the information about the director.


#### Used Technology

Flask is used to run the website and the server uses SQL to retrieve the requested data from SQLITE database. Bootstrap was used for designing the pages. JavaScript make the website more dynamic and user-friendly. It let the browser communicate with the server behind the scene and provide the autocompletion features, and react to the click of the suggestions to submit the form automatically for the user, and shows icon according to the conditions. Python takes care of data visualization part. Data_vis.py makes a graph with the retrieved data and store it in the graph storage. Manage_graphs monitors the storage, to delete old files if it gets too big.

I used Sqlite3 module instead of cs50 SQL module this time. Cs50 SQL module makes it easier for us. I researched how to use sql on script without the help of SQL, and added indexes to make sql query faster.

#### Features to be Implemented

Unfortunately, the database is too big to run online for free, but if I am able to do so in the future. I would like to add feature showing the often searched directors. Right now the graph is saved as a picture and showed on the page. Sometimes the movie titles overlap depends on the data retrieved. I would like to check Pyscript to make interactive graphs on the page to avoid those situation. About the database, it's not up-to-date so, I would like to make a new database to 2022 with the IMDb API.

#### Conclusion

This was my final project of CS50. As I am a self-taught programmer/data analyst, it was a great opportunity to see how one of top schools teaches computer science and programming. It was really exciting to build up something integrating all the technology we learned through the course at the end. I have one website for my portfolio with Django. I will definitely develop it with the knowledge I gained from this course and of course I'm going to check up the other CS50 courses. Most likely the CS50 web development is my next course.
