# Entry 2
##### 11/30/20

In this point of time, I should be ready to start planning out my project.
As for the websites I have been using, I've been on Repl for testing my tool,
[Firebase](https://firebase.google.com/).
I will show snips of my code later in this blog. It is recommended to use my repl as (reference)[https://repl.it/@SamLee5/Testing-FireStore#index.html]
for better understanding, although not necessary.

My stage in the Engineering Design Process is probably stage 4, which is to **plan the most promising solution**.
I've already thought of the possible solutions to my problem of unorganization. Obviously I wanted something more efficient
and something that won't take a lot of time to use. I've narrowed my way to down the idea that this app allows you to press
things on screen and the user will just need to fill in necessary information (i.e. Page numbers or amount of minutes needed to read).

The tool that I've been focusing on is Firebase and I will continue to use this tool. Specifically I've been using its [FireStore](https://firebase.google.com/products/firestore)
feature. This is probably the key feature of the tool that helps me store and retrieve data. In addition, my project that I'm working on is a
homework and assignment tracker that is efficient because it allows quick user input that would automatically be placed into a list
as a reminder.

In terms of skills, I've learned how to **embrace failure** and **debugging** when tinkering with my tool. Initially when I tried to
install Firebase into my Web App, I went through some errors. Although I was pretty new with the tool, just by looking at the code,
I realized that I had installed an older version of the database. I simply debugged this by switching from a Realtime-Database into the new
Cloud Firestore.

<!--![Code Installation](../images/code-install.png)-->
``` javascript
<script src="https://www.gstatic.com/firebasejs/8.1.1/firebase-app.js"></script>
<script src="https://www.gstatic.com/firebasejs/8.1.1/firebase-firestore.js"></script>
```

Represented by the first script, it's allowing the **Firebase App** to deliver the tools
almost as if it's downloading it into the html file.
The second code is similar, however, it's downloading a different set of libraries which is the **Fire Store**
, a type of database run by Firebase. In short, the first line is necessary in order for anything to work
, while the second line opens up the database to allow the information coming from the html to actually go through.



To give a little context for the following piece of code, I've created a simple textbox that can be typed in into the
website. After pressing the "Submit" button right after it, the text entered will be sent into the database that I have created in Firestore.


``` javascript
function submitData() {
  var someText = document.getElementById("mainText").value;

  db.collection("Users").doc("Number").set({
  name: someText
  })
  console.log(someText);
}
```
In this function, I have defined `someText`. Note that `someText` is a **variable** that connects with text written in the textbox in the html.
"db" is the variable of the database, which I then go into the "collection," then "doc" which ultimately becomes set by the text
in the textbox.
To sum it up, I'm basically setting the child of "Numbers" which is the child of "Users" to be `someText`.


[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)