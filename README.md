# Twitter NLP Web Application

- Access the [Twitter API](https://developer.twitter.com/en/docs/twitter-api/getting-started/getting-access-to-the-twitter-api)
   - Apply for elevated status to allow higher volume of tweets per month. 
   
 - `models.py`: creates schema for SQLite database using [SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com/en/2.x/)
 
 - `predict.py`: Looks at two given users' tweets, vectorizes them with [Spacy](https://spacy.io/models/en) 
 
 - `twitter.py`: Accesses twitter api to get add new users to the database from given user input. Checks to see if user is already in the database. Denotes current tweet ID for later reference when checking for updates. Also provides `vectorize_tweet()` function which applies Spacy vectorizations. 
 
 - `app.py`: Provides deployed Flask URL endpoints for viewing user tweets, resetting database, adding users to the database, updating existing users' tweets, and comparing users to generate a prediction for output.


![Twitter](https://pbs.twimg.com/profile_images/1488548719062654976/u6qfBBkF_400x400.jpg)
