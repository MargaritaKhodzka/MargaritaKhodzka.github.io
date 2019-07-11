---
layout: post
title:      "My Favorite Activities: adding JS frontend to the  Ruby on Rails app"
date:       2019-07-11 03:17:22 +0000
permalink:  my_favorite_activities_adding_js_frontend_to_the_ruby_on_rails_app
---


The goal of this project is to add dynamic features to my previous Rails application through JavaScript and a JSON API. My application makes it possible for users to create a list of activities and then managing them by adding associated locations. A user can rate and add a description for each activity happening at a certain location. The index page for all locations is public and can be viewed and contributed to by all users. The reason for it is that there can be multiple people visiting Central Park in New York or The Louvre in Paris. To keep the application database fast and compact, it makes sense that duplicate locations are not created for multiple users. 

I started by adding 'active_model_serializers' gem to the Gemfile and generating location, activity and location_activity serializers to be able to render JSON views and create model associations. Location_activity is a joint table through which locations and activities have many_to_many relationship.

The first requirement was to translate JSON responses from the Rails app into JavaScript Model Objects using either ES6 class or constructor syntax. The Model Objects must have at least one method on the prototype. I used a constructor function to outline the properties of a Location: id, name, city, state, zip_code, location_activities, and activities. There are two methods on the prototype in this app - formatIndex() and formatShow().

The second requirement was to render an index page ("a list of things") via JavaScript and an Active Model Serialization JSON Backend. I decided that a list of Location would be a perfect example of that. The page displays a list of all locations created by users. Once a user clicks on "Locations" link, an API call is made to /locations route and returns a JSON object. Locations are formatted in an unordered list, with links to their perspective show pages.

The third requirement was to render at least one show page ("one specific thing") via JavaScript and an Active Model Serialization JSON Backend. When a user clicks on an LI from the Locations index page, (s)he is re-directed to a Location show page. On this page, all information is listed, as well as all activities that are happening at this location. Here, the app dynamically renders a serialized 'has_many' relationship (a location has many activities through location_activities).

The last requirement was to render a form for creating a resource that is submitted dynamically and displayed through JavaScript and JSON without a page refresh. I added a link to the nav bar to add a new location. After the form is completed and submitted, the new location is appended to the app-container as a Location show page.

This has been the most challenging section of the curriculum and the hardest project so far. It gave me an opportunity to do a lot of research and really learn how to filter through and find the necessary information on the web. It helped me to understand JavaScript better and practice abstract thinking.

Feel free to fork and contribute to my repo on [Github](https://github.com/MargaritaKhodzka/rails-my-favorite-activities-js-frontend).
