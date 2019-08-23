---
layout: post
title:      "React-Redux project - Travel App"
date:       2019-08-23 01:49:28 +0000
permalink:  react-redux_project_-_travel_app
---


For the final project, I created a Travel App that has Destinations and Categories tables in the database. A destination has many categories, and a category belongs to a destination. I got this idea from my travel plans. Locations around the world have more to them than we might think at first. When we think of Rio de Janeiro, the beach comes to mind. When we think about New York, we think about Manhattan with its skyscrapers. However, there are many more activities in these cities travelers might not be aware of. The idea behind the app is that people will contribute by adding new destinations and categories (activities) in these destinations. Users can also add destinations to their "Bucket List" and "Visited" lists to keep track of places they want to go to and places they've already traveled to. 

This app has React-Redux frontend and rails API backend. Rails API  handles the data persistence, and I used fetch() method within actions to GET, POST, PATCH, and DELETE data from the API. The client-side application handles the display of data with minimal manipulation. I made use of react-router and proper RESTful routes for easy data manipulation and consistency. Redux Thunk middleware was used to write functions that add asynchronous logic and dispatch actions when certain conditions are met. 

The app has clean minimalist styling, and I used reactstrap and custom CSS to achieve this look. 

This has been the most difficult project for me both technically and morally. Since this is the final project, I wanted to apply all the knowledge I acquired at Flatiron School. Abstract thinking is the main skill, and I am still learning how to abstract logic and make applications and files reusable. Knowing the meaning of `this`, `state`, and `props` is another work in progress for me and something I have to be constantly aware of. I am glad I became more comfortable and adventurous with CSS and reactstrap framework while working on this project. 

Overall, I am satisfied with my work although I have a few more features in mind that would make it better. I will continue working on and improving this application.

