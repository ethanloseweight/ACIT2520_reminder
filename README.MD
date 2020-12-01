# Reminder App
## Developed by Rony Tran, Oliver Yan, Oliver Si, Ethan Liu
  
# Description:

```
reminderApp2 2
 ┣ controller
 ┃ ┣ auth_controller.js
 ┃ ┗ reminder_controller.js
 ┣ public
 ┃ ┣ index.html
 ┃ ┣ script.js
 ┃ ┗ style.css
 ┣ views
 ┃ ┣ auth
 ┃ ┃ ┣ login.ejs
 ┃ ┃ ┗ register.ejs
 ┃ ┣ partials
 ┃ ┃ ┗ navbar.ejs
 ┃ ┣ reminder
 ┃ ┃ ┣ create.ejs
 ┃ ┃ ┣ edit.ejs
 ┃ ┃ ┣ index.ejs
 ┃ ┃ ┗ single-reminder.ejs
 ┃ ┣ .DS_Store
 ┃ ┗ layout.ejs
 ┣ .DS_Store
 ┣ database.js
 ┣ index.js
 ┣ package-lock.json
 ┗ package.json
 ```
Sprint 3:

1. When you click between "Reminder List" and "Create" in the navbar, it should correctly toggle the "active" link with the color filled black. (Hint: check out res.locals) [INCOMPLETE]
 
 How we could try and implement: Use local variables scoped to the request.
  
2. You should include the ability to have logged-in users staying logged in through a cookie session. Despite having sessions, you will still use a fake database for authentication. (You will see during lecture how to work with cookies and sessions for log-in)[INCOMPLETE]
  
  How we could try and implement: [The user provides a username and password in the login form and clicks Log In.After the request is made, the server validate the user on the backend by querying in the database. If the request is valid, it will create a session by using the user information fetched from the database and store them, for each session a unique id called session Id is created ,by default session Id is will be given to client through the Browser.]

Sprint 4:
1. You could accomplish this by having a page which shows all registered users, and a button next to each user that says: "Add friend". When you click this button, it should add that friend to your friends list in your fake db, and you should be able to see all of their reminders on your reminder list page. You can delete them as a friend from the same page, and their reminders should no longer show up on your page.[INCOMPLETE]

  How we could try and implement: [When add friend button is clicked, the user should be sorted into a dictionary with all their user informations and their reminder lists. Then the reminder list should be update base on this dic from fake database. If the delete friend button is clicked, the database will delete corresponding user dic and the reminder list will be update.]
  
 2. Every user in your application needs to have a field in their database called profile picture.[INCOMPLETE]
 
  How we could try and implement: [We will use the website unsplash to get pictures of people]
  
 
