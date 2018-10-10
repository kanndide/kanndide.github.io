---
layout: post
title:      "React-Redux with Rails API"
date:       2018-10-10 07:06:11 -0400
permalink:  react-redux_with_rails_api
---


### It's finally here.
The final project. Just as the title suggests, it's a React-Redux frontend UI with a Ruby on Rails API backend. You shouldn't be surprised to hear that I may have tried doing something that was a bit more that was necessary for the project, but that's how you learn, right? I mean, that's how I learned to swim. You think you can trust someone, then they don't catch you. First, you panic. Then, like it was something you always knew how to do, you swim to the surface... Only to hear the voice (the one belonging to the Benadict Arnold that didn't catch you in the first place) saying, "good job! Now swim to me."  

Ok. That may not be the best metaphor for learning how to code or the best way to teach your 3 year old kid how to swim, but I learned two valuable lessons that day:   
1.) How to swim (aka how to learn under pressure).
and
2.) Not to trust anyone.
Just like jumping in the water feet first, with no depth check, and exactly how I started this bootcamp, I ended it the same way. Let's paint the setting for this project before I dive into the experience. Imagine a small concrete room, located in Baghdad, Iraq, a 2013 13' Macbook Pro, and *The Carter V* playing through the portable speaker, because it's high time it finally dropped and why not give this story a sountrack. Oh, and a 35 day vacation in China closing in fast.
Back to the subject, the one about this project. Remember?
Remembering back to the glory days of DOS, loading games floppy disk after floppy disk, an utilizing the command prompt for everything, I decided to make a simple text-based RPG. Simple. The word that caught me off guard. I figured I would just build a basic Rails API with a super simple way to create the user, characters, stats, etc. and then rig up the React frontend and be done with it. Super easy. 
The Rails portion of the project wasn't too hard. I decided to use Devise to manage user authentication and creation. There was a bit of a learning curve with it and about 2 hours of looking through the documentation for it but it seemed simple enough. I went with the JWT-Devise, since it was an API and generated my Rails app with the API flag to get rid of the unnecessary bloat in it. I created my migrations with the idea that it would basically just store all o the persistable data belonging to the user and their character(s) and then React would take care of everything else.
I used `create-react-app` to generate the app and I dug in. I found out pretty quick that we never really discussed user creation and stuff in the React-Redux sections but I knew the basic idea from Rails and Javascript, so no big deal. That was wrong. I ran into quite a bit of push back getting that portion to work. I found some solid guides, readmes, and tutorials on setting up a React frontend UI and did my best to pull what I could use and make it my own for this project. I set up the app container, the user container. I started getting the Redux middleware in order. Things looked good. Then I stalled for a while actually getting it communicate with the API the way I needed it too. I also had to figure out how to use the JWT token and everything else that comes with logging into an API. I also discovered this thing called CORS (cross-origin resource sharing) that hung me up until I figured out a way around it with `Rack::Cors` (and then later become stumped by it again). I could probably write an entire post on that, so I won't go into detail here.
After I finally got the user portion of the project completed I realized that I had already surpassed the requirements for the project. Yay me!
I added in functionality for all of the next portions I need to work on to continue this learning project. I inted to keep working on this idea in my spare time. It seems like there is a lot to learn from it and their is value in knownledge, even if no one besides myself and a friend I coerce play it. Right now the project succesfully allows a user to register themselves with it, log in, and show the user their profile (information) and start to show them the characters they have created and their location in the story. Next, character creation. After that is the fun part, getting the game ready to play. I haven't figured out yet whether I need to actually persist the data (text) for the story in the backend or have it stored for rendering in the frontend. I want to game to play as a simple, almost decision based, style text rpg. 
This was actually a fun project to work on. Everything else that I said I disliked about Javascript has gone away as I started to get a grasp of React. I have a long way to go but I am finally feeling like I can get the hang of this.
Until next time.

