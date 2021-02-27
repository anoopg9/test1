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

## Deploy to Heroku
*Don't do the Heroku step for assignments, you only need to deploy for Project 2*
1. Create a Heroku app: `heroku create --buildpack heroku/python`
2. Add nodejs buildpack: `heroku buildpacks:add --index 1 heroku/nodejs`
3. Push to Heroku: `git push heroku main`

## Techinical Difficulties
1. Updating the Name to the spectator list after getting Player X and Player O
2. UseState functionality to update it's state
    To better understand https://daveceddia.com/usestate-hook-examples/
3. Also Reseting the Board was tough.

## Things still needed/That could Improve
1. Still need help on storing users into playerX or playerY or spectators
2. Highlight the winner 
3. Need Logout button after user login