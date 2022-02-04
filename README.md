# Flask Simple CRUD app

## Get started

1. `pip3 install virtualenv`
   - Just execute one time
2. `virtualenv env`
   - We create a common env for collaboration between collages.
3. `.\env\Scripts\activate` (Windows)
   - We are activating the environment and show in console: `(env) C:\workspace\flask-simple-crud>`
   - Then we can install requirements executing into env: `pip3 install flask flask-sqlalchemy`
4. We create the starting point: `touch app.py`

5. Execute app: `python app.py`

6. Import db with python and create database:

   - In other command line we enter in the env: `.\env\Scripts\activate`
   - execute python shell: `python`
   - import db: `from app import db`
   - create database: `db.create_all()`

## Heroku

1. Sign up in Heroku and install Heroku CLI.
2. type in the console: `heroku login`
3. Enter user and password

## Gunicorn

We install gunicorn as a server where execute our app

`pip3 install gunicorn`

We specify this server in `Procfile`

Then we freeze requirements: `pip3 freeze > requirements.txt`

## Create a instance in heroku

`heroku create flasksimplecrud`

We push our code in Heroku remote git:

1. `git remote -v`
2. `git push heroku main`
