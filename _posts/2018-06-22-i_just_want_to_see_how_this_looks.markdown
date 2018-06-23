---
layout: post
title:      "Class Roster Sinatra App"
date:       2018-06-22 23:16:09 -0400
permalink:  i_just_want_to_see_how_this_looks
---


I started this project, in my typical fashion, with loftier ideas than I ended up with. It still holds the same basic principle of my original idea, but it doesn’t house all the features I wanted. Honestly though, it doesn’t need them. The project isn’t about how much you can put into it, just whether or not you understand what they want you to understand. Hopefully I do.

This project had a fairly simple, straightforward goal. Make an app in Sinatra that isn’t twitter or a blog… Well, Sinatra seems suited for two basic things: blogs and twitter.
 
It took me a bit you figure out what to use it for that wasn’t one of those things. After talking with my wife, who is a teacher, I figured I would go with the class roster idea. Why not, right? I could be reaching here, but it seems like even if I name it differently and claim it isn’t a blog or twitter it still has the same structure and concept. It just has different names for objects.

I started out strong with the app, recording my coding walkthrough (30 minutes) and almost completely finishing it in that time frame, or so I thought. I basically had all the files in place and the basic bones. It took me a couple more days to finish out all of the views and the routes. I could have probably done it all in one day, but it gets kind of tedious and tedious can get kind of boring. Plus, I work.

The object of the app is very simple. A user is a teacher. You can sign-up and login. Once you are signed up and logged in you can create a course. Once a course is created you can add students to it. That’s it! You can see your courses on the user’s home page and get into the details utilizing links on the site. Some links only appear if you are logged in and most features only work if you are logged in and the objects belong to the user.

I am really not sure what else to say about this particular app/project. The controller routes and views became kind of fun at points. It was nice to be able to build them out without having a reference up all the time. I guess if you do it enough it begins to stick.

There are several types of associations or relationships with the object models in this app. Having two many-to-many relationships took a little thinking but in the end it all worked out.

I am going to stop stalling. Check out the project on my [GitHub](https://github.com/kanndide/class-roster-app).
