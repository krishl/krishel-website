---
layout: post
title:  "Potatotainment"
date:   2017-01-16 06:10:38 -0500
Author: Krishel Lasam
categories: 
tags: [project, ruby]
comments: false
---


This Ruby gem lists all currently trending shows and movies along with their respective details based on real-time check-in data from Trakt.tv.

When first approaching this project, I first thought if any of my most commonly visited websites were suitable for this project. I decided on basing this project on data from a website called Trakt.tv, which helps users keep track of movies and shows that they are currently watching or have watched in the past.

I decided on using data from four different categories:

- Currently Trending Shows 
- Most Anticipated Upcoming Shows
- Currently Trending Movies
- Most Anticipated Upcoming Movies

Each category lists out the appropriate shows/movies based on live user data.

![](https://puu.sh/toaf9/9d07f95698.png)

A show/movie is considered "Trending" based on the total amount of people who are currently "checked in" on the show/movie's page. The "checked in" status remains for the entire length of the total runtime for the show/movie.

A show/movie is considered "Most Anticipated" based on the total amount of people who have added that particular show/movie onto their "watchlist". 

Since this is based on real-time data and the shows/movies on each list are always changing, I had to accommodate for that by identifying the common URL pattern for each entry in order to be able to proceed onto the detail view for each show/movie.

The URL pattern that shows follow is:

- Spaces are replaced by dashes
- Special characters are deleted

As for movies, the pattern is as follows:

- Spaces are replaced by dashes
- Special characters are deleted
- The release year of the movies are included at the end of the URL

![](https://puu.sh/toamY/27c40c3bdc.png)

The detail views of each show/movie include publicly available data such as title, release year, description, genre, runtime, country, and language. A detail page for an upcoming movie may not always have a runtime length or genre available yet, since the movie may not be released until the following year (or longer). This program was written to adjust for these discrepancies by first listing out the most commonly available detail categories before listing out the variable details.

A short video demo of this gem can be viewed [here](https://youtu.be/WzMI70dfPSE).

The repository for this gem can be found [here](https://github.com/krishl/trending-entertainment-cli-app).

The gem itself is published on rubygems.org, available [here](https://rubygems.org/gems/trending_entertainment_cli_app).
