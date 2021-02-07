# Requirements

Before we start we need to install this

1. Requires Flask
*	sudo pip install flask
    https://flask.palletsprojects.com/en/1.1.x/quickstart/
2. Requires request
* sudo pip install requests

3. Requires python-dotenv
*  sudo pip install python-dotenv

4. Requires Spotify API
*	Requires Client Key and Secret Key to access the API
*	https://developer.spotify.com/documentation/web-api/quick-start/
*	https://developer.spotify.com/documentation/web-api/reference/#category-artists
*	

## Once this process is done follow these steps to run the program
1. In cloud9 or any IDE ,first create templates and store ‘Index.html’ and add some line to see if it is running. After doing this run “python app.py”
2. This should successfully render the HTML file with the help of jinja.
3. https://hackersandslackers.com/flask-jinja-templates/


### Technical Issues that came up during this project
* Running the program in different port like example (port 8000)
https://api.spotify.com/v1/artists/{id}/top-tracks
* Adding  “?market=US” after the top tracks gave me an error for the params. Instead I had to make a separate variable PARAMS ={“market”: ‘US’}
* Another Issues tha I got is index slices when reading through JSON file. To fix this and read clearly I used JSON Formatter

    https://jsonformatter.org/json-pretty-print


### Additional Features
* Add more HTML and CSS to actually make the border filled with Iphone color
* User Search for the artist instead of hard coding the artist (Down below Link should help us with that)
 
https://developer.spotify.com/documentation/web-api/reference/#category-search
