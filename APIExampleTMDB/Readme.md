# **The Movie Database Example App**
## *A simple Android client for The Movie DB in Material Design.*

This project is an Android app which displays data from [The Movie Database API](http://api.themoviedb.org/).

[Video of App](http://i.imgur.com/rY2ZTYl.gifv)

In this assignment I had to provide 3 main user features:
**Goals**

1. White Action bar.

2. Screen 1 - Search for movies, 
  *A search button that reveals the text enter and submit button. 
  *Show list of movies found in the same screen.
  *Lazy Load future sets of data from pagination added to the list.
  
3. Screen 2 - Show movie details when a list item is clicked
  *Open images of a movie

**Notes: **
I wanted to display my knowledge of JSON and Parsing Apis by using 2 different methods to get the api information from TMDB. 
First I used [Apache.HTTP](https://mvnrepository.com/artifact/org.jbundle.util.osgi.wrapped) to make a request for the user's search query and page number.

Then I used [Retrofit(2)](https://github.com/square/retrofit) to get individual movie id data in the recyclable's adapter. 
I chose to use [Picasso](https://github.com/square/picasso) to load all images from the internet in order to handle asynchronous image downloading for a more smoother experience. In the [APIExampleOMDB](https://github.com/Tc2r/APIs/tree/master/APIExampleOMDB I used Glide to do the same).

For UI  I wanted to go for a more [Material Design](https://material.io/guidelines/), implementing my own custom action bar which also serves as the search box. I used CardView with a slight shadow, and Google's Palette library to match the CardView theme to that of the movies downloaded. 
