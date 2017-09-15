---
layout: post
title:  "Working on my Rails Project"
date:   2017-09-15 04:46:47 +0000
---


For my Rails project, I decided to create a travel bucket list app, where users could add new destinations to their list and add categories to these destinations. Categories and destinations have a many-to-many relationship through a join table so that destinations can have many categories, and categories can have many destinations. Users can mark destinations as 'visited' once they visit the locations they've listed on their bucket list.

As usual, the most difficult thing for me was to create migration tables and model associations, especially so with a joint table. I was considering destination_categories and user_destinations. At some point, I had both of these tables, which broke everything I had build at that point. Then, I decided to go with destination_categories table as users can have any destinations regardless.

Another difficulty I experienced was establishing Omniauth connection to Facebook. As I work on Learn IDE terminal, the link to my app keeps changing every day, which means that I have to update the Site URL every day. But I realized that only after a day of trying to reinstall the whole connection routine in my app a couple of times. That is something I will have to keep in mind every time I was to use this app.

The new thing I got to add and work with is bootstrap. Once I had the app functioning, I added some navbar, form, and button design. I struggled with it as well, as it was something completely new for me.

Overall, I am satisfied with my project. I think I will keep working on it just to perfect the layout and views.
