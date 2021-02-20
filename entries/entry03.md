# Entry 3
##### 02/22/21

In my Freedom Project, I have at this point of time, started to create something that is potentially relevant to creating a Homework Organizer.
After getting back into firebase, I've gotten a better understanding of the tool, and I was able to create something simple yet important.
As for my sources, I have looked over the firebase documentation again, however this time, I've looked into specifically on how to
[add data](https://firebase.google.com/docs/firestore/manage-data/add-data) and [get data](https://firebase.google.com/docs/firestore/query-data/get-data).
I will show snippets of my mini-project as I was tinkering with firebase later. All code shown will be referenced from my [repl](https://repl.it/@SamLee5/Testing-FireStore#script.js).
Also I will link my [Cloud Firestore](https://console.firebase.google.com/project/firestore-testing-9095c/firestore/data~2Fusers~2Fusers-name) which is where data gets inputted into from my repl.

At the moment, I would consider myself between stage 4 and 5 of the Engineering Design Process. I haven't completely created a protocol, however, I did create something that potentially can be used in my Freedom Project.
I would say that I've planned on how to create my web application, however, I haven't solidified on my choices in building it. In terms of what I have created so far, I made a mini web application where it
asks the user for their name and their assignment that needs to be done. I'm able to then save their data and access it. Because I haven't created a full protocol for this Homework Organizer, my next steps in the
Engineering Design Process is to fully create a working web application that takes user input and stores it.

With our live sessions on Zoom, I've been getting more comfortable with learning the basics of Javascript. I incorporate these little things in my mini project, such as using "if statements" and making variables which I've learned in
class.

Here are some snip-its of code that I have in my mini-project

```javascript
    var userName = prompt("What's is your first name?")
    var userDoc = usersRef.doc("users-name")

    var userAssignment = prompt("What's your assignment today")
```
In the code above are some basic variables that I set up in order to store user input. I used some simple javascript to subsitute DOMs which I haven't explored yet in this point of time.
These variables are created to be used later

```javascript
    if (userName != null && userAssignment != null){
        userDoc.set({
        name:  userName,
        assignment: userAssignment
    },{merge: true} )}
```
In the code above, there's the simple ```if statement``` which basically makes sure that there's information inputted before saving it.
In the code INSIDE of the if statement is something new I've learned from Firebase. It first references the document, then it stores data with its field and value. In this case, I'm
making the name set to ```userName``` which is the variable I set up earlier, and I've set the assignment field with a value of ```userAssignment``` which I also set up earlier. This
saves the code into Firestore which then can be grabbed out later.

```javascript
    userDoc.get().then((doc) => {
        var assignment = doc.data().assignment
        document.write("Assignment: " + assignment)
    })
```
In the code above, it's a block of code that essentially allows the data to be grabbed from the Firestore Database and written into the html portion of the web application. It was a little hard to comprehend at first,
however, all it's doing is basically waiting for the document from the Cloud firebase to be written back to the script, which then the script can manipulate the data within it. In this case, I've simply used
```document.write``` to write the "Assignment" and it's correlating value into the actual HTML.

Lastly, I've acquired some new skills throughout the Freedom Project. Specifically, I've learned about Time Management and Organization. These two skills are incredibly useful and needed. I've learned to time manage more efficiently.
Obviously, there would be time to break and time to work. In making my mini-project, I've learned that I shouldn't cram information in my head. What works best for me is looking at the documentation or guide, then taking a break from it
before looking at it again. This helps for me especially since it's more efficient than trying to understand something by spending more time as my mind cannot comprehend it. This also brings me into the skill of organization. I've learned to take notes
while being organized. In order to do this, I've actually cleared my repl and started from scratch. The previous file I had was unbearable as it was a mess. To make it more organized, I've started using comments as notes which helps me organize
it far better than I've done before. It makes it clearer and easier to access my scripts.




[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)