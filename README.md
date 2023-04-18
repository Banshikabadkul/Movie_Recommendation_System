# WH050_Brainstorm_Brigade
# Movietrix - Movie Recommendation System

## Overview
Movietrix is a movie recommendation system that offers generalized recommnendations to every user based on movie popularity, genre, and year. 
The model also give personalized recommendations based on the user's choice of genre and cast.
Finally, the system suggests similar movies have a higher probability of being liked based on the movie selected by user. 

## Features
1. Sign-up and Sign-in functionality. ✔️

2. Forgot password (resetting password) functionality. ✔️

3. OTP validation. ✔️

   `The user receives a mail containing OTP for validation before resetting the password.`

4. Restrictions and validations on the sign-up page, sign-in page, forgot password functionality, OTP validation page, and reset password page. ✔️
   
5. The User’s credentials are stored in the database. ✔️
  
6. Completely responsive frontend. ✔️

7. A total of 4 types of recommendations:
  * Recommended movies based on the user's chosen genres and casts. ✔️
  * Most popular movies based on different genres. ✔️
  * Most popular movies based on different years. ✔️
  * Recommended movies similar to the user's selected movie. ✔️
  
8. Movie details and trailer linked for each movie. ✔️

9. Watch a movie option. ✔️

10. Option to like or dislike a movie. ✔️

11. Client-side session tracking. ✔️

12. Continious deployment. ✔️


### Restrictions and validations on the sign-up page, sign-in page, forgot password functionality, OTP validation page, and reset password page
* All fields not filled
* Email account already registered (sign-up), Email account not registered (sign-in)
* Incorrect password, OTP incorrect
* Email address not entered, OTP not entered, new password not entered



## Tech Stack and Softwares used
1. `Frontend` : HTML5, CSS3, JavaScript, BootStrap, jQuery
2. `Backend` : Python flask
3. `Database` : PostgreSQL, SQLite3
4. `ML model` : Jupyter Notebook
5. `IDE` : PyCharm
6. `Version Control` : Git
7. `Deployment` : Heroku



## Libraries and Toolkits used
`Python` : NumPy, Pandas, ast (Abstract Syntax Trees), pickle

`ML` : ntlk (Natural Language Toolkit), sklearn (scikit-learn)

`SQLite` : sqlite3, SQLAlchemy


## Recommendation Algorithm
For recommendations of similar movies, a content-based recommendation system. For recommendation, the system takes into account movie titles, genres, starring cast, keywords, overview, and the director. I have implemented Cosine Algorithm after the vectorization of movies. 
It is achieved by using Annoy (Approximate Nearest Neighbors) mechanism. Resource for Annoy: https://github.com/spotify/annoy


## Future Scope
* `Like/Dislike` : The option to like or dislike a movie adds the movie to the user's like/dislike list. As of now, I am just accumulating the data. This can be further extended by using the like/dislike list to recommend movies to the user.

* `Watch Movie` : The watch movie option currently displays the same movie intro for all the movies. In the future, it can be customized according to the movie selected.

* `Collabrative Filtering` : The model currently uses a content-based recommendation system. It can be converted into a hybrid system by adding a collaborative filtering mechanism.


