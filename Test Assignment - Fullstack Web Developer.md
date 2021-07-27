# Test Assignment - Fullstack Web Developer

## 

### Assignment

- Create a simple "Reminders" web application using Python & JavaScript.
The goal of this app is to deliver notifications about upcoming events from user's todo list. 
You can use any means of delivering notifications (email, chatbots, sms APIs, etc).
Also, you're not limited in choice of Python or JavaScript frameworks. 
However, we expect a working solution with clean and maintainble architecture.

- Application functionality:

	- As a user:
		- I can add/remove/delete the text reminders.
		- I can set date and time of reminder.
		- I receive text reminders about upcoming events on my email or chat. 
	
	  You can use any means of delivering notifications (email, chatbots, sms APIs, etc)

### Tech stack:

- Python - any web framework, i.e, Django, Flask, FastAPI, Odoo.
- Javascript - any UI framework or library.
- GIT - the solution should be posted on any public hosting.
- Docker - the solution must be provided with correct Dockerfile and docker-compose. 

### UI/Design

- Application mockups are located in the directory "screens".
- There's no goal to make a pixel-perfect solution. You're free to use any UI library as long as it works.


## Specification

### 1. Reminders list

- As a user, when on the home screen, I see:

	- Header (AppBar) and application body:

		- AppBar:

			- On the left side: Bold text "Reminders" 
			- On the right side:  Green button "➕" 

			  <a href="screens/00_header.png" target="_blank"> Example(header.png)</a>

		- Application body:

			- When loading:

				- In the middle of the application body I see the text "Loading..." on white background

				  <a href="screens/02_main_screen--loading.png" target="_blank"> Example(screens/02_main_screen--loading.png)</a>

			- When I have due reminders:

				- I see the list of text reminders:

				  <a href="screens/01_main_screen.png" target="_blank"> Example(screens/01_main_screen.png)</a>

			- When I do not have due reminders:

				- Following text on white background: "You have no reminders yet! It's time to add one"

				  <a href="screens/02_main_screen--empty.png" target="_blank"> Example(screens/02_main_screen--empty.png)</a>

			- When server error:

				- The text "Server error" on white background

				  <a href="screens/03_main_screen--error.png" target="_blank"> Example(screens/03_main_screen--error.png)</a>

	- 

### 2. CRUD Actions

- In application header I see the button " ➕"

  <a href="screens/00_header.png" target="_blank"> Example(screens/00_header.png)</a>

	- When I click the button " ➕",  I see the form with following elements:

	  <a href="screens/04_add_form.png" target="_blank"> Example(screens/04_add_form.png)</a>

		- Textarea
		- Button "Set Date"
		- Button "Set Time"
		- Button "Add"
		
		- When I click "Set Date", I see:

		  <a href="screens/05_edit_date.png" target="_blank"> Example(screens/05_edit_date.png)</a>

			- A calendar widget, where I can pick the date
			- Button "Save"

				- When I click "Save" - the caledar closes and the date shows in the parent form

		- When I click "Set Time" , I see:

		  <a href="screens/06_edit_time.png" target="_blank"> Example(screens/06_edit_time.png)</a>

			- A time-picker widget
			- Button "Save"

				- When I click "Save" - the time picker closes and the time shows in the parent form

		- When I click "Add":

			- The form closes
			- In the begining of the reminders list, I see the new reminders

		- 

- Application body I see the list of reminders

	- Each reminder has the button "⌄"
	
		- When I click "⌄", I see a dropdown menu with action "Edit":

		  <a href="screens/07_actions_menu.png" target="_blank"> Example(screens/07_actions_menu.png)</a>

			- When I click "Edit", I see following edit form:

			  <a href="screens/08_edit_reminder.png" target="_blank"> Example(screens/08_edit_reminder.png)</a>

				- When I click "Save", the reminder data updates
				

### 3. Notification delivery

- As a user, I receive text reminders about upcoming events on my email or chat. 

	- When the reminder is delivered, it doesn't show on web application UI
	- The application should attemt to deliver notification up until successful response from delivery service.



## Good luck!
### 


