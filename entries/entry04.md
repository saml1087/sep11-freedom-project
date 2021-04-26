# Entry 4
##### 4/26/21

Through the course of this entry, I will go through the process of creating the DOM portion of my Freedom Project. As my project is based on saving/documenting assignments that the user is needing to keep track of, I needed to make the application able to process the user's input and display it in a nice "list" format. In addition, I've done more Firestore testing which could potentially be added into my application.

Here is the **timeline** that focuses on what I did this week.

![timeline](entrys-snips/entry04-screenshots/timeline.png)

Throughout this project, I've done my testing on my demo-website which is [here](https://ide-28ce95ffd3744292bda1b0e1ac9b55a5-8081.cs50.ws/index.html) for reference. My testing done with Firebase will be located [here](https://replit.com/@SamLee5/Testing-FireStore#script.js). Some addition sources I've used as reference were firebase's [documentation](https://firebase.google.com/docs/firestore/manage-data/add-data) on adding data and a simple [keycode grabber](https://keycode.info/)

At this point of time, I'm at the **create a prototype** stage of the Engineering Design Process. I've been working on the HTML portion and the DOM portion of my web application in the previous weeks. I've been able to add some CSS to make my web application a little more pleasing to the eye. In this entry, I will be going over the DOM that I have added as well as some additional Firebase tinkering that will be soon added to my demo-website. In the coming weeks, I'll be soon finishing adding aspects of my tool, Firebase, into my application as well as testing my protocol and try to prevent any source of bugs and errors.

As I was coding in script.js in my demo-website, I ran into an error. (Code Below)

![error1](entry-snips/entry04-screenshots/error1.png)

The first three lines are there for the set-up. I've created three separate variables that grabbed using the `querySelector()` some HTML as well as the first variable that uses `createElement()` to make a list component. Then I continued on with the Button feature. How would I be able to make the application listen for an event? Well, it was obviously needing the `addEventListener` for `click`. Now the slight mistake that I had was actually a typo.

![fixerror1](entry-snips/entry04-screenshots/fixerror1.png)

![fixerror1.1](entry-snips/entry04-screenshots/fixerror1.1.png)

As you can see above, I've made a simple typo error because the names were mismatched. It's very common that these mistakes happen, and it's very possible that a whole program wouldn't work because of one typo. Obviously, it should be easy to fix, but I would like to emphasize that these errors are common and they do happen.



[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)