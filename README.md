Movie Recommendation System 🎬🎥🎞️ </h1>

## Objective:
Our recommendation system's main goal is to filter and predict only those movies that a user would like based on the individual data provided by the user. The different implementations applied to this project are the Content-Based Model and the Collaborative Filtering Model. At first, we worked on a content-based model to predict the movies for recommendation, but the downside of the model is that it predicts the top 10 movies based on the genre provided by the user and not by their preference. Based on the above reasons, which provided the same movie set for all users since it was based on genre, we moved onto the next model, which is Collaborative Filtering. This is a model used to create a recommendation based on the user's rating history (i.e., movies rated in the past). Collaborative recommender systems aggregate ratings or recommendations of objects, recognize commonalities between the users on the basis of their ratings, and generate new recommendations based on inter-user comparisons. Collaborative filtering is more efficient in this project than in the content-based model. To work on this project, take a pull or fork the code from this repository and modify it as per your requirements.   


## About data source:
 As per the data source, all the data files contain 1,000,209 anonymous ratings of approximately 3,900 movies made by 6,040 users who joined the service in 2000. There are three data set files added inside the dat_files folder for this project. The file format of the data set file is .dat format. These .dat format files are further processed and converted into CSV files and saved in the root directory, then those files are further used in the project. The reason for choosing this dataset is that it has a reasonable number of rows in each file. It also had both categorical and continuous data. It also helps us achieve our target goal of predicting movies based on user preference.

### User.dat file description

user_id :: gender :: age :: occupation :: zipcode
				
The data source provided the information that all demographic information is provided voluntarily by the users and is not checked for accuracy.  Only users who have provided some demographic information are included in this data set.

- UserIDs range between 1 and 604 and also serves as the foreign key for User.dat and Ratings.dat file

- Gender is represented by an "M" for male and an "F" for female.

- Age is chosen from the following ranges "Under 18" to "56+" years of age:

- There are 21 different occupations collected by the data source. 

### Movies.dat file description

movie_id :: title :: genres 

- MovieIDs range between 1 and 3952 and also serve as the foreign key for the Movies.dat and Ratings.dat files.

- Titles are identical to titles provided by the IMDB (including year of release)

- Genres are pipe-separated | in the same column:

- Some MovieIDs do not correspond to a movie due to accidental duplicates entries and/or test entries.

- Movies are mostly entered by hand, so errors and inconsistencies may exist.

### Ratings.dat file description

user_id :: movie_id :: rating :: timestamp

- UserIDs range between 1 and 604 and also serve as the foreign key for User.dat and Ratings.dat files.

- MovieIDs range between 1 and 3952 and also serve as the foreign key for the Movies.dat and Ratings.dat files.

- Ratings are made on a 5-star scale (whole-star ratings only).

- Timestamp is represented in seconds since the epoch as returned by time (2).

- Each user has at least 20 ratings.


## Online dataset link

[Link](https://grouplens.org/datasets/movielens/1m/) - Link to the data set.
