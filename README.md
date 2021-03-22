# [Netflix - Movie Recommender and EDA with Plotly](https://github.com/chanchanngann/netflix_recommender/tree/master)

### Summary
* Part 1. Used Plotly to do the EDA to explore the TV shows and Movie data on Netflix, answering some inspiring questions:

   1. What are the target audience in different countries?

   2. Understanding what content is available in different countries (the US vs. Korea)

   3. Is Netflix has increasingly focusing on TV rather than movies in recent years?

* Part 2. Created a movie recommender to suggest 10 movies on Netflix that are similar to the movie-in-interest.

***

### Part 1 - EDA
#### Program types on netflix
![](https://github.com/chanchanngann/netflix_recommender/blob/master/plot_image/1_tv_to_movie.png)

Movie to TV contents ratio is 70:30 on netflix.

#### Top 20 countries with most content
![](https://github.com/chanchanngann/netflix_recommender/blob/master/plot_image/2_top20_countries.png)

Rank #1 is the US, followed by India and the UK. The US is more than 3 times of India in programs count.
The result is quite insteresting for Movie vs TV program split. Movie got higher share in US, but opposite result seen in Japan, South Korea, Taiwan - TV contents showed higher share.

#### Q1. What are the target audience in the top 10 countries?
![](https://github.com/chanchanngann/netflix_recommender/blob/master/plot_image/3_target_audience.png)

In general, Asian countries (South Korea, India, Japan) have lower proportion on adult contents (26% - 44%) while western countries have higher proportion on adults contents (42% - 79%). For the extreme cases, Spain has almost 80% occupied by adults content while india only has 26% adults content. Most content available in india is kids programs.(72%)

More about kid content in India:

The world of cartoons and kids’ content has caught the fancy of many over-the-top (OTT) streaming players in India. The top six to ten platforms including Netflix, Amazon Prime, Hotstar, Voot, Sony LIV and Eros Now — besides YouTube — have capitalised on the growing appetite for content created for kids or children in India. source: [here](https://inc42.com/features/toons-and-beyond-indias-ott-players-take-baby-steps-into-edutainment-kids-content/)

#### Q2. What content is available in different countries? Let say US vs Korea?
![](https://github.com/chanchanngann/netflix_recommender/blob/master/plot_image/4_genres_korea.png)
![](https://github.com/chanchanngann/netflix_recommender/blob/master/plot_image/5_genres_us.png)

For South Korea, most contents are romantic tv shows (40%), followed by Crime TV shows (13%). While for the US, the program types are quite diverse, main programs cover Dramas, documentaries, comedies, children movies,...etc.

#### TV vs Movie Trend - Release Year
![](https://github.com/chanchanngann/netflix_recommender/blob/master/plot_image/6_released_yr.png)

#### TV vs Movie Trend - TV vs Movie Trend - Year_added to Netflix
![](https://github.com/chanchanngann/netflix_recommender/blob/master/plot_image/7_added_yr.png)

#### Q3. Is Netflix has increasingly focusing on TV rather than movies in recent years?
![](https://github.com/chanchanngann/netflix_recommender/blob/master/plot_image/8_tv_to_movie_by_yr.png)

The share between TV vs movie was similar in 2016 , then movie showed a big jump from 58% to 71% in 2017. Movie share reached the highest in 2018, occupying 74% of total. Yet, starting from 2019 TV share increased gradually, movie share dropped to 65% in 2020.

Probably due to covid-19, less movie launched and led to decrease in movie share?? Or simply because auidences' increasing interest in TV shows?!

___

### Part 2 - Movie Recommender

By entering a particular movie name (which is available in the dataset), the movie recommender is able to return 10 similar movies.

