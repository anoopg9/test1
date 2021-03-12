# Flask and create-react-app

## Requirements
1. `npm install`
2. `pip install -r requirements.txt`

## Setup
1. Run `echo "DANGEROUSLY_DISABLE_HOST_CHECK=true" > .env.development.local` in the project directory

## Run Application
1. Run command in terminal (in your project directory): `python app.py`
2. Run command in another terminal, `cd` into the project directory, and run `npm run start`
3. Preview web page in browser '/'
 
## Create a new database on Heroku
1. First login to your heroku `heroku login -i`
2. Create a new Heroku app: heroku create
3. Create a new remote DB on your Heroku app: `heroku addons:create heroku-postgresql:hobby-dev`
(If that doesn't work, add a -a {your-app-name} to the end of the command, no braces)
4. See the config vars set by Heroku for you: `heroku config`. Copy paste the value for DATABASE_URL
5. Now create a .env and store your database url and export it.
6. After following this steps we must run some command in python
    `>> from app import db`
   a>`>> import models` 
    a>`>> db.create_all()`
    a>`>> admin = models.Person(username='admin', email='admin@example.com')`
    a>`>> guest = models.Person(username='guest', email='guest@example.com')`
   a>` >> db.session.add(admin)`
    a>`>> db.session.add(guest)`
    a>`>> db.session.commit()`

## Deploy to Heroku
*Don't do the Heroku step for assignments, you only need to deploy for Project 2*
1. Create a Heroku app: `heroku create --buildpack heroku/python`
2. Add nodejs buildpack: `heroku buildpacks:add --index 1 heroku/nodejs`
3. Push to Heroku: `git push heroku main`

## Techinical Difficulties
1. Updating score as winner and loser in database and displaying in the Front End.
2. The problem I faced is that it's emiting infinte types as winner and loser which crashed my databse
3. I still have dificulties about useEffect.


## Things still needed/That could Improve
1. Highlight the winner 
2. Need Logout button after user login