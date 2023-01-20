# DOCUMENTATION
# COFFEE APP
This project is an small app to test a third party authentication service like Auth0. It simulates an app for a coffee bar where manager and baristas has different permissions to take actions in the app. The code is written under the Pep-8 principles.

# GETTING STARTED
The stack of the application is Flask for the backend and Ionic for the frontend. The database is SQLlite. The project was developed internally so the url is refering a localhost owned by Udacity.

# API REFERENCE
# GET '/drinks'
Fetches a list of all the drinks that are recored in the database. Request arguments: None. The description is short.

"drinks": [ { "title": "Water3"}]

# POST '/drinks'
Fetches the detail of a drink. Request arguments: None. This route display drinks with its recipe.

"drinks": [ { "title": "Water3", "recipe": {"name": "Water", "color": "blue", "parts": 1}}],

# GET '/drinks-detail'
Fetches the detail of a drink. Request arguments: None. This route display drinks with its recipe.

"drinks": [ { "title": "Water3", "recipe": {"name": "Water", "color": "blue", "parts": 1}}]

# DELETE '/drinks/int:question_id'
Delete the drink in database Request arguments: id of the drink (integer value) When clicked it sends a delete to db. It response the id of the deleted drink and when done it a true success.

{ "deleted": 1, "success": true }

# PATCH '/drinks/int:question_id'
Upload the drink in database Request arguments: id of the drink (integer value) When clicked it sends a update te to db. It response the id of the updated drink and when done it a true success.


# DEPLOYEMENT
Frontend
Install Node and NPM This project requires on Nodejs and Node Package Manager (NPM). If you haven't already installed Node on your local machine, see the instructions here: Before continuing, you must download and install Node (the download includes NPM) from Nodejs.com. Install project dependencies After confirming you have NPM installed, navigate to the frontend directory of the project and run.

npm install npm start

The frontend folders got public folder with images and media. And src folder where you can find the components and stylesheet.

Backend
Need to install dependencies. Check for updated packages.

pip install -r requirements.txt

Primary dependencies: Flask, SQLAlchemy, Flask-CORS.

To start the server, positioned in backend/src folder:

export FLASK_APP=api.py 
flask run --reload

# TEST

You can test in Postman with {} udacity-fsnd-udaspicelatte.postman_test_run.json

AUTHORS
Juanan Jiménez

ACKNOWLEDGEMENT
All the work wasn't possible without the help of Udacity mentors.
