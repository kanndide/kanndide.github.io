---
layout: post
title:      "Rails Project App"
date:       2018-07-20 18:50:22 +0000
permalink:  rails_project_app
---


It seems like something always happens when I start a project. It’s like I step into a worm hole and time starts doing some funny, relative things. I blew through the Rails section in no time at all, finishing everything but the project in about 11 days. I thought, “Man, I am going to knock this project out in, like, two days. This must be some kind of record.” Then, the worm hole called life and work happened. It took me about that many days or more to finish the project and get me to this point, writing the blog. 

This project is similar to my Sinatra project, but done in Rails. It has added features that I wanted to add to the last one, better styles, and was a little easier to put together thanks to Rails having easily learned patterns and structures. 

The idea of this project is that a User can sign in, create a profile and be able to find schools and lectures and create a schedule so they can keep track of everything. I eventually want to add in some other features like a chat room for each lecture, email capability for the teacher, etc. 

I did my own user authentication because I didn’t want to learn Devise while I was working on a project but that would also be one of the changes I would likely implement as well.

This app has one user models with three different levels of privileges. The standard user, a student, can create and account or log in with Twitter (no Facebook because I don’t have Facebook and there was no way to do the OAuth tokens without an account) and then create their profile and start finding schools and lectures to create their schedule. They can edit their own account and add lectures but that is about the extent of their privileges.

The teacher user can create, edit and delete lectures. This user is one step above the student user. 

The admin user has all the privileges they need. The admin is the only one that can mark a user as a teacher or as another administrator. They are also the only user that can create schools. The idea behind this is that each level only has a certain ability and can’t foul up the rest of the app and create a whole bunch of unnecessary items within the database. The admin also has the ability to edit or delete any other user, lecture or school, in case some fouling happens anyway.

I suppose there is also a super user (me) who can do whatever he wants on the back end whenever he wants. Rock on.

That basically covers the app. I did my best to utilize standard routes and naming conventions throughout it but there were a couple of instances where I believe I didn’t. I did my best to keep the controllers lean, having most of the actions being done by the models and using them only for giving information to the views. I also did my best to remove anything that wasn’t needed and keep the code DRY. That being said, I will find out where I went wrong when I do the review for this project.

All and all the process wasn’t that bad. I enjoyed working with Rails more than I did Sinatra. Rails makes it easy (subjective term). Most of it seemed to stick in my memory. As I went on I had to use the Google machine less and less. 
I have been having to battle with horrible internet recently as well. As I am typing this my walkthrough video is slowly uploading to youtube. Thanks to an impromptu, country-wide firewall and internet traffic consolidation in Iraq I have been having to do everything through a VPN. That and the already pond-like speeds of the internet here have made this a very slow process.

Luckily, I am finally finished.

Check out my repo at [Github](https://github.com/kanndide/classroom-manager)
