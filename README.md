![Movie Analysis Banner](images/movie_analysis_banner.jpg)
# Microsoft Movie Analysis

**Author**: Bijal Saija

## Overview

Microsoft has decided to create a new movie studio and requires more insight into which types of films are doing best at the box office. This project uses descriptive statistical analysis of data gathered from the IMDb website to gain insight into which combination of genres or which are the most popular genres in today's generation over the last few years. Three separate datasets were used for this analysis to gain insight into which combination genres of movies topped the total gross, had the top average ratings movie genres, and best studio's top-grossed genres. The results of the top 20 combination genres in highest-grossed movies, top rating movies, and highest-grossed movies in the last 15 years combination of Action, Adventure, and sci-fi, with adventure being present in the majority of the top 20 of the 3 categories. My recommendation for which type of Movie to produce would be Action, Adventure, or sci-fi as this is the most predominant combination in the analysis by top-grossed movies, there were 260 unique genre combinations in this data set after cleaning. I recommend that Adventure and Action paired with either Animation or Fantasy is a successful combination which I have analysed by top studio's top 10 movies. In total gross, the combination of Adventure, Animation, and comedy also faired well which would be my third recommendation. Adventure was a strong genre for popular successful movies.

## Business Problem

Microsoft wants to produce movies that are going to be successful to make profits, they want to know which types of movies are the most successful. To answer that question, domestic and Foreign Sales data was analyzed to see the most financially successful genres, along with the average rating and popularity over the years for each type or genre of movie to see how popularity compared with financial success.


***

## Data

The data analyzed came from the IMDb website. IMDb (an acronym for Internet Movie Database) is a popular worldwide online database of information relating to all movies, television programs, video games, and streaming content online. I used 3 files from IMDb to answer the question of which genres were most successful, mainly focusing on the Domestic and Foreign Gross sales along with average ratings given and release year of popularity genres.

After checking the information on each table to see column names and null values, I joined the two datasets, df_titles_basic_info and df_ratings together using the 'tconst' column as it was a unique identifier creating a new data frame called inner_merge. I then joined the dataset tn.movie_budgets with the new data frame using the title as the unique identifier, creating a combined new dataset called df49 using 'title' & 'movie'.

Checking the information on the new data frame complete_df, I then cleaned up the null values by removing them, tidied up the "Domestic Gross' and 'Foreign Gross' columns, and converted them to units of $ millions for easier readability and analysis. The columns"studio", "original title", and the original domestic and foreign gross columns were deleted as they were not required to carry out this analysis.
***

## Methods

The data analyzed came from the IMDb website. IMDb (an acronym for Internet Movie Database) is a popular worldwide online database of information relating to all movies, television programs, video games, and streaming content online. I used 3 files from IMDb to answer the question of which genres were most successful, mainly focusing on the Domestic and Foreign Gross sales along with average ratings given and number of votes received. Describe the process for analyzing or modeling the data.

***
After checking the information on each table to see column names and null values, I joined the two datasets, imdb.title.basics and imdb.title.ratings together using the 'tconst' column as it was a unique identifier creating a new data frame called inner_merge. I then joined the dataset tn.movie_budgets with the new data frame using the title as the unique identifier, creating a combined new dataset called df14.

Checking the information on the new dataframe df14, I then cleaned up the null values by removing them, tidied up the "Domestic Gross' and 'Foreign Gross' columns and created totl_gross column converted them to units of $ millions for easier readability and analysis. The columns "original title", and the original domestic and foreign gross columns were deleted as they were not required to carry out this analysis.
***

## Results

3 of the above graphs, top 10 rating genres,top 10 genres of top grossed movies and top genres of last 15 years clearly show that Adventure, Action and Sci-Fi combination are most successful in Domestic and Foreign Gross Sales and also in the average rating given. Its clear also to see that the adventure genre is popular across the board especially when elements of animation, action and or comedy are also included.

The 4th graph showing line graph of top 5 genres over the years top grossed genre action as solo genre.

To improve confidence in the results next time I would:-

Include the movie classification This could have narrowed down the target audience the most successful movies were aimed at i.e PG etc.

Will check number of votes in different age group, see if audience tastes change by age.



***

***



## Conclusions

This analysis leads to three recommendations regarding types of movies that are successful:-

Movies with the genre combination Action, Adventure & Sci-Fi topped the leaderboard in both Domestic and Foreign Gross Sales, this combination is obviously a hit at the box office worldwide, make this the first type of movie to produce for success.
Movies with Adventure, Animation and Comedy were the next most successful in top rated movies, use this combination as the next or alternative type of movie to produce.
Movies in the top 20 recent years yielded slighly different results but Action, Adventure and Sci-Fi combination did come out 1st still.
Adventure genre seems constant in all the above graphs so must be a key element of any movie to be produced.
Questions to consider:

Limitations-Could the same movie be classified into different genres by different audiences? Who classifies the genres for each movie? Can the classification of genres be improved to provide a more benchmark approach?
Future analysis could include the movie classification ie PG, MA etc to see which audience the most successful movies were made for.
***





## Repository Structure

Describe the structure of your repository and its contents, for example:

```
├── README.md                           <- The top-level README for reviewers of this project
├── microsoft_movie_analysis.ipynb      <- Narrative documentation of analysis in Jupyter notebook
├── microsoft_movie_analysis.pdf        <- PDF version of project presentation
├── zippedData                          <- Data repositories sourced externally
└── images                              <- Both sourced externally and generated from code
```
