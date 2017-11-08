---
layout: post
title:      "Travel Bucket List, part 2"
date:       2017-11-08 03:41:36 +0000
permalink:  travel_bucket_list_part_2
---

I can't believe I am almost done with the Rails project with JQuery Front End. I felt like it would never end and I would never find a solution to the bugs I had. At some point, I really wanted to give up. At first, I was quite enthusiastic about it - the guidelines were clear and I thought I knew how to meet them. Silly me. 

First of all, I couldn't decide on which JSON object I wanted to append to the DOM, whether this could be a comment, a visited destination review, or a category. The indecisiveness made my progress so much slower! I build, reversed, and re-build the app so many times that I have lost all understanding of where I was, what has been done so far, and how do I move on from here. Finally, I have decided to add new categories to a destination show page.

Originally, in my Rails project, I had Destinations and Categories with a many-to-many relationship. However, I category could be created only with a destination, not independently. So, while destinations didn't have to have categories, all categories needed to have at least one destination.

The fact that now I could create a category in the destination form, while editing a destination, and now via Ajax post request got me and the controllers all confused. With a lot of help from the instructors, I managed to sort it out, but I still think my code could have been cleaner.

I am meeting the project requirements by rendering the category index page on the destination show page while displaying the has-many relationship in JSON. New destinations are being fetched and rendered via JQuery/Ajax by clicking the "Next Destination" button on the show page. With that, appropriate categories are rendered on each destination's page.

I read through the main requirements so carefully and so many times, but, literally, the second line of the overview has skipped my mind. I did use remote: true in this application, although we are not supposed to. Had to change that later on, just when I thought I was done. 

Lessons learned from this experience: read the instructions more carefully (!!!) and do not despair - in a couple of months, this project will probably seem like a piece of cake.
