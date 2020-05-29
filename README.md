# Movie-Recommender-System
The following project deals with a simplified version of movie recommendation system which are deployed in various web services these days from your favorite Netflix, Amazon Prime etc. The effort has been made to implement the basic idea behind these recommendation systems. The basic idea behind this project is to find correlation among various independent variables (Movie Ratings) and matching them to predict the desirable movie for the user.

# Source of Dataset
The source of the movie ratings dataset used in this project is obtained from https://grouplens.org/datasets/movielens/ . The description of the dataset are as follows -:
100,000 ratings and 3,600 tag applications applied to 9,000 movies by 600 users.
The dataset is cleaned prior to applying correlation techniques and Null values are taken care of.

# Tools and Libraries Used
1) Jupyter Notebook
2) Pandas Library (for Data Manipulation)
3) Matplotlib (for Visualisations)
4) Seaborn (for Visualisations)

# Methodology 
First we select a sample movie that the user has watched earlier and given good ratings. In my project i have selected two random movies belonging to two different genres. The first movie is Star Wars (1977) which is a Science Fiction movie, and the second movie selected was Liar Liar (1997) which is a comedy movie. 


![](Images/Liar_Liar.jpg) ![](Images/StarWars.jpg)                                                  



Our main objective is to suggest similar movies to the users who have watched atleast one of the two movies mentioned above.

The individual ratings of these two movies is selected from the dataset and stored into two different pandas DataFrame.

Then we try to find the correlation of these two movies separately with the remaining of the movies in the datset stored in the form of matrix and compare the results obtained. The movies which were observed to be highly correlated with the ratings of our sample movies were suggested to the users. Whereas movies with comparatively lower correlation score were not suggested.

On doing that there was an anomaly occuring due to the large difference in the ratings given to different movies. For ex - one such case is when a single movie is watched by less people (maybe 1 or 2) but still managed to get a high rating which is just based on two observations. Therefore suggesting such movies to users will defeat the purpose of recommndation systems. Hence, suitable techniques were used in the project to address this issue.

# Conclusion
Hence, a Recommendation System model was implemented with some of the basic concepts related to correlation and statistics. 

# Further Scope of Project
The basic model of this project can be further extended to generate sophisticated recommendation results to users which will be more accurate and extensively based on user's choice. Some of the further developments includes taking into account the Age, Sex, Region, Language preferences factors to prepare a model that would predict very relatable movie choices to its users.
