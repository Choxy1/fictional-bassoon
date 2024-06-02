## MICROSOFT MOVIE ANALYSIS



Microsoft Studios is excited to venture into the creative arts and movie production industry. To support the head of Microsoft Movies, this project aims to analyze box office performance and identify trends in successful films. The key questions we will investigate include:

Genres
Which genres perform best at the box office?

Directors
Who are the top-performing directors at the box office?


Studios
Which studios achieve the highest box office success?

## Data Understanding

We have two data sources: a SQLite3 database containing movie information across various tables, and CSV files from imdb

## Database

The database includes five tables, of which three are pertinent to our analysis: Movie Basics, Directors, and Movie Ratings. To align with our objectives, I joined these three tables on the common feature movie_id to create a consolidated table, ensuring to select only relevant features and avoid duplications. The selected features are movie_id, original_title, primary_name, runtime_minutes, genres, averagerating, and numvotes. I then transformed this consolidated table into a Pandas DataFrame using the Pandas library for easier data manipulation.

# CSV FILES

The first CSV file includes movie titles, studios, gross earnings in domestic and foreign currencies, and the year of release or production, with a total of 3,387 records.

The second CSV file contains various features such as genre IDs, movie ID, original language, original title, popularity, release date, title, vote average, and vote count, encompassing 26,517 records.

Finally, budget information and other related data come from the budget CSV file, which has 5,782 records. This dataset includes six features: ID, release date, movie title, production budget, domestic gross, and worldwide gross.


## Data Preparation

# Data Cleaning
 We remove the data thet we dont need from the datasets

 ## Data Merging


 # Data Exploration
 Two important features I consider necessary for the dataset are:

-Profit

This represents the difference between revenues and the budget.


-Month Produced

This feature will help us identify the month in which movies were produced.
