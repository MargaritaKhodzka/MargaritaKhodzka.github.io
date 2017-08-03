---
layout: post
title:  "My Sinatra MVC application  "
date:   2017-08-03 18:42:25 +0000
---


For my first CLI project, I had a hard time coming up with an idea. That is why, once I began the Sinatra part of the curriculum, I started thinking about the project and, finally, made my mind up around the time I was working on the Fwitter project. While working on labs, the first thing I did was run migrations and build models because this information and structure are already given to us. For this project, I couldn't make a decision on how the tables supposed to look like and what columns they should have. So I run created migrations only by the end of the second working day. Then, had to make some changes to the tables. So that, I would say, was the most difficult part. Just in terms of organization.

I work at an etiquette school as a personal assistant and manage day-to-day inquiries and schedule. For my notes, I use the Notes app on my Mac, which can get messy and unorganized pretty soon. For this project, I decided to create an app that would keep track of our clients, the courses they take, and their booking status. For that, I have four controllers - Application, Users, Clients, and Courses - and three models - Client, Course, and User. I, as a user, can sign up, log in, and log out, and cannot perform any tasks unless I am logged in. Or any user, for that sake. 

Clients have courses, and courses belong to clients. Users have many clients. I can create a new client, edit, see client info, and the full list of clients. I can view and edit courses, as well as create a new one. However, I prefer to create a new course when I register a client as all of our courses are bespoke and the names vary depending on the client's needs. That is why I wouldn't want to create a new course independently from a client. Although it is good to have that option. I can access the list of all courses in the command line, '/courses', or by clicking on the course link that appears on a client's show page.

I had a little problem adding error messages, since I haven't done that before - we used redirect logged_in? method to redirect to the login page. So that was something new.
