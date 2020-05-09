# Java-Build-a-recommendation-system

## Description

It is the project of Coursera's Java programming "Build a recommendation system" course.

Here we are asked for building a capstone project by taking a look at the features of a recommender engine. I chose how to read in and organize user, ratings, and movie data in my program. 

In this capstone, I wrote code to recommend movies based on different criteria, criteria based on user ratings of those movies.

The person who runs the project will be able to make recommendations by filtering based on genre, or co-stars, or by any other criteria.

I designed and wrote classes to implement a recommendation engine that makes recommendations along the lines we've just discussed. My program could make recommendations from many sources. Food, movies, books, or more. It just depends on the data that you read in.

### Let me give you a detailed description about what I did

So basically I devided my project into four parts:

#### First step:

I created a sequence of recommendation programs as part of this capstone. The first step in creating programming recommendations was to get data about the items that can form the basis of the recommendations my program will generate. I wrote programs to read the data into structures so that my program can access and process to make recommendations. Although I won't using Yelp or Netflix data to generate my recommendations, I am using Twitter data about movie recommendations, to write my own recommender program. I am using recommendations for movies that have come from Twitter posts, via a project called MovieTweetings. 

The data I used is stored in CSV files. 

I read the data and store the rating movie data in collections my program will access to create recommendations. I started with simple storage techniques, and as I started creating more sophisticated recommendations, I used more efficient data structures, using the software design principles I've learned in the specialization that Coursera provided.

I used Plain Old Java Object, or POJO, to store the movie data. The movie.java class mirrors the CSV file storing the movie data.

That CSV file contains one line of comma separated value data for each movie. Each line of the CSV file stores eight items of information about each movie. The first item is an IMDB or internet movie data base ID number, for the movie. The title of the movie is the next one on the line, followed by the year in which the movie was made, a country in which the movie was made, though sometimes there is more than one country. Then the genre of the movie, such as comedy, action, adventure, horror or more. There can also be more than one genre listed with the movie.

Then there are the movie's directors, followed by the length of the movie in minutes. I read the CSV file and use the POJO class that Coursera created, to store data for each movie. The **Movie.java** class has a constructor and several getter methods for accessing data about the movie. Once a movie object is created it doesn't change. The get methods include, get title, get I.D., get year and more to access information about each movie. I read this data using the edu.duke file resource class and the Apache CSV parser.

