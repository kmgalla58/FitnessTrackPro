# Instructions To Run Project
1. Install Docker Desktop
2. Clone repo into IDE
3. Run in terminal: docker compose up --build
4. Enter this URL in the browser: localhost/login

# Env Variables
Create a .env file in the root directory of the project and include these variables:
- MYSQL_ROOT_PASSWORD="pumping_iron"
- MYSQL_DATABASE="fitness_track_db"
- MYSQL_USER="ftp"
- MYSQL_PASSWORD="pumping_iron"

- DB_ENGINE=mysql
- DB_HOST=database
- DB_PORT=3306
- DB_WEB_PORT=8083
- DB_CHARSET=utf8mb4

- JWT_SECRET=(generate this value using this Javascript crypto method: crypto.createSecretKey())

# User Guide
## Signup & Log In
When a new user navigates to the page, click "Sign up". The user will be navigated to the sign-up page where they can create a new account. When a user successfully creates an account, a toast popup should appear confirming this and the user will be redirected back to the login page. From here, they can enter their credentials and hit "Log In". Upon successfully logging in, the user will be directed to the view workouts page.
## View Workouts
Here the user can view the list of all their past workouts. If the user wants to sort this list by a specific column, they can click on the column header. If they hover their mouse over a column header, three dots will appear. If the user clicks on this, a popup will appear and if they click on "Filter", they can search for specific entries. If a user wants to **delete** a row(s), select the checkbox for that row(s) and hit the trashcan button below the list. A user can add a new workout to the list by selecting the "+" button below the list. A popup will appear where the user can enter the name and date of the workout. If the user hits "Submit", the popup will close and the list will now display the new workout. If a user clicks on the row itself (not the checkbox), it will direct them to the edit workout page for that specific workout. If the user clicks the "Logout" button in the top left of the page, the user will be logged out and directed to the login page. If the user clicks the "View PRs" button in the bottom left, they will be directed to the **Personal Bests** page.
## Edit Workout
This page allows users to edit the name and date of a workout, and add, edit, and delete workout items. To add a workout item, click the "+" button below the list. A popup will appear where the user can select an exercise from a dropdown menu, and then enter the sets, reps, and weight performed. If the user hits "Submit", the popup will close and the list will now display the new workout item. You can edit the fields of each workout item by double-clicking on the field you want to edit. If you want to remove an item, click the checkbox for that item and then hit the trash icon below the list. Once you are done editing, click the "Save" button. If successful, a popup should appear saying that it was successfully saved. YOUR CHANGES WON'T BE SAVED IF YOU DO NOT HIT THE SAVE BUTTON. From there the user can navigate back to the view workouts page by selecting the home button in the top left of the page.
## Personal Bests
Here, the user can view their all-time best for each exercise they have ever done. When a user saves workout items, if an exercise has been done for the 1st time, the system will log the weight done for that exercise in the personal best list. If the user has done an exercise before and the weight is greater than their all-time PR, the system will update that exercise in the personal best list. This list can be sorted and filtered in the same way the view workouts list can. Users can navigate back to the view workouts page by selecting the home button in the top left of the page.
## Downloading Fitness Tracker Pro
Depending on your browser, there should be an option to download Fitness Tracker Pro. After clicking this prompt/button, FTP will now appear on the home screen of the user's device.
