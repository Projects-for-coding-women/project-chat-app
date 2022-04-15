## Project Chat App

### The goal of this project is to practice working with JavaScript and the DOM, creating an interactive app

We will use HTML, CSS, and JavaScript for our project. This project is for students who are comfortable with JavaScript and working with the DOM.

**Basic functionality:** we want our chat app to show a random (automated) chat message from the CodeWomen 'user', as a reply to the dynamic messages that are typed in the message field by the WomanDev 'user'. These messages have to be shown on the screen in a sequence, with the first message at the top and every new message added at the bottom. The random automated messages take 2 seconds to appear, showing a spinner on the screen during that time.

A simple example looks like this (spinner shown in the image on the right):  

<img src="./images/screenshot1.png" width="300" />              <img src="./images/screenshot2.png" width="300" />

---

### For more advanced students

1. Create a new folder on your local computer with the name: project-chat-app
1. Track your code with Git by using git init in the terminal
1. Create an index.html file with the general template code
1. Create a main.js file. Copy the array with strings from the `replies.js` file and paste it at the top of your main.js file, or import the file into main.js
1. Create a style.css file
1. Link the JavaScript file to the HTML document so that the JavaScript code will be able interact with the HTML
1. Add a link to the css file in the HTML
1. Add **The Unexpected Chat** inside the `<title>` tags
1. Add the welcome message as shown in the example (only the first message is hardcoded)
1. Create a template message element with:
    1. an icon value. The icons to be used are in the images folder: codeWomen.pngfor the automated messages and woman_dev.png for the external user
    1. a name value (either CodeWomen or WomenDev, or use your own name if you like)
    1. a message field where the messages entered by WomenDev will be shown
1. Create the input field in the footer where new messages are typed by the user (make sure the footer stays at the bottom of the screen, even when there are only one or two messages)
1. Create a submit button for the message input. The submit event has to:
    1. grab the content of the message input field
    1. place this into a new WomanDev message element
    1. add this at the bottom of the message trail
1. Make sure the Enter key also has this same submit functionality
1. The message trail has to move upwards so that you always see the last message on the screen, a bit above the input field
1. The submit event also has to 
    1. create a new automated CodeWomen message with a random hardcoded message
    1. place this as a reply under the last WomanDev message
    1. have a time lag of two seconds to imitate the time needed to write a real message
    1. activate a spinner on the screen during these two seconds
    1. block the screen during these two seconds so that the user cannot enter messages
1. Use a function to randomise the messages that are automated replies, and that also prevents a reply from being used more than once
1. Test your code by writing at least ten new messages that generate reply messages - the replies should be unique

---

### For graduates

1. Build this project as React app
1. Use create-react-app, create components and write the code for the functionality explained above
1. Challenge yourself: deploy the app on Heroku or Netlify
1. Create a method that a user can use their own avatar and name instead of the WomanDev
1. Make it into an attractive, professional looking app


---

## Please note:
If you want to download a project on your local machine, do not fork it but clone the repo locally, on your computer. After that, create a new repo in your own GitHub account *with exactly the same project name*, and link the local repo to the remote repo in your GitHub account (see below). Why should you clone and not fork? It will show the project as **your own project** and not a fork of someone else's project. You can use it as a project for your portfolio.

You can connect a local project to a new, empty GitHub repo [as follows](https://docs.github.com/en/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line). We can do this together during a CodeWomen coding session: it is very good to know this so that you can start a project locally and afterwards link it with a remote GitHub repo.

If you clone the project without forking it, you will have to change the 'remote origin' repository after cloning. Check the remote of your local project using `git remote -v`. You will probably see:  
`origin  https://github.com/CodeWomen-Barcelona/some-codewomen-project.git (fetch)`  
`origin  https://github.com/CodeWomen-Barcelona/some-codewomen-project.git (push)`

To link your local project to your own GitHub repo, you need to change the remote origin. Have a look at this article: https://devconnected.com/how-to-change-git-remote-origin/. With `git remote -v` you can again check if remote origin has been reset and now shows the name of your GitHub account.

PS: if you work for a company that has a corporate social responsibility policy and wants to support women in tech, then here is the link to the [fundraising overview of MigraCode](https://docs.google.com/spreadsheets/d/1Zs-Mmi39bcjVw2U-iEQWSHSjkb-EmET-j1WB2oJF45Q/edit#gid=0).

---
