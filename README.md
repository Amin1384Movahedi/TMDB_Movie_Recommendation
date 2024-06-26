# TMDBM Movie Recommendation

<h2>About Dataset</h2>
<p> Background: What can we say about the success of a movie before it is released? Are there certain companies (Pixar?) that have found a consistent formula? Given that major films costing over $100 million to produce can still flop, this question is more important than ever to the industry. Film aficionados might have different interests. Can we predict which films will be highly rated, whether or not they are a commercial success? </p>
<p> This is a great place to start digging in to those questions, with data on the plot, cast, crew, budget, and revenues of several thousand films. </p>
<h3>Data Source Transfer Summary</h3>
<p> We (Kaggle) have removed the original version of this dataset per a DMCA takedown request from IMDB. In order to minimize the impact, we're replacing it with a similar set of films and data fields from The Movie Database (TMDb) in accordance with their terms of use. The bad news is that kernels built on the old dataset will most likely no longer work. </p>
<p> The good news is that: </p>
<ul>
   <li> You can port your existing kernels over with a bit of editing. This kernel offers functions and examples for doing so. You can also find a general introduction to the new format here. </li>
   <li> The new dataset contains full credits for both the cast and the crew, rather than just the first three actors. </li>
   <li> Actor and actresses are now listed in the order they appear in the credits. It's unclear what ordering the original dataset used; for the movies I spot checked it didn't line up with either the credits order or IMDB's stars order. </li>
   <li> The revenues appear to be more current. For example, IMDB's figures for Avatar seem to be from 2010 and understate the film's global revenues by over $2 billion. </li>
   <li> Some of the movies that we weren't able to port over (a couple of hundred) were just bad entries. For example, this IMDB entry has basically no accurate information at all. It lists Star Wars Episode VII as a documentary. </li>
</ul>

<p> <strong>References:</strong> </p>
<ul>
   <li> <a href="https://www.kaggle.com/tmdb/tmdb-movie-dataset" target="_blank">TMDb Movie Dataset</a> </li>
   <li> <a href="https://www.themoviedb.org/documentation/api" target="_blank">The Movie Database API</a> </li>
   <li> <a href="https://www.imdb.com/interfaces/" target="_blank">IMDb Interface</a> </li>
</ul>

<h3>Calculating Benefit per Cost or B_C for all records in our dataset</h3>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/Benefit-Cost-Ratio-Formula.jpg" alt="B_C Formula" />

<p>To calculate the benefit per cost obtained from each film made, we have to divide the income by the cost, and if the result is less than one, it means that the film was not profitable, and if the result is more than one, it means that the film was profitable.</p>
<p>We can subtract the results by one and then compare it with zero.
Now we can easly determine which movie is profitable or not profitable.</p>
<p>It is possible to examine the films that were not profitable and find the reason for their non-profitability, the mistakes in the film and the director's mistakes in order to avoid these mistakes in order to make a new film.</p>

<h3>How much does it cost to make each genre of film?</h3>
<h3>How much is the benefit of each movie genre?</h3>

<p>By drawing a bar graph, it can be understood that the highest cost is required to make a movie with the action genre, and the lowest cost is required to make a movie with the "tv movie" genre.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/Budget_per_Genre.png" alt="budget per genre chart" />

<p>Now we will draw a bar chart for the profit obtained from the production of each genre of film.</p>
<p> By looking at the chart, we can see that the most profitable genre is the horror genre, followed by the mystery genre and then the comedy genre.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart2.png" alt="B_C per genre chart" />

<h3>Top twenty companies that spend the most money on film production and earned the most revenue.</h3>

<p>Now let's take a look at the twenty companies that spend the most money on film production.</p>
<p>In the beginning, the Prime Focus company is the first, after that the Silver Bullet Productions and the third company is Blind Wink Productions Company.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart3.png" alt="Top twenty Companies that spend the most money on film production." />   

<p>Now, by looking at the chart of top twenty companies that earned the most revenue between all of the movie companies, we can realise that Colorado Office of File, Television & Media is the first and the second company is Quebec Production Services Tax Credit and the third is Prime Focus</p>
<p>Due to the fact that the company has made the main focus of the second investment in the production of films, but it has not had the highest income and it has been the third company in generating income.</p>
<p>the Silver Bullet Productions company and Blind Wink Productions Company, although these two companies are among the twenty companies with the highest investment in the film industry, they are not among the twenty companies with the highest revenue generation.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart4.png" alt="top twenty companies that eaned the most revenue." />

<p>Even though these three companies were among the most profitable companies, but they were not among the most profitable companies, it may be because they had more expenses in addition to the large income they had.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart5.png" alt="top twenty companies with highest B_C" />

<p>Blumhouse Productions and Solana Films, these two companies have been among the most profitable companies, but they are not among the top 20 companies with the most profits, it may be because they have relatively lower income than the rest of the companies, but their costs are much lower than the rest of the companies have spent.</p>

<h3>The directors who spent the most money for the production of the film and made the most profit with the production of the film</h3>

<p>Let's take a look at the directors who cost the most to produce films.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart6.png" alt="directors with most spent budget" />

<p>Steven Spielberg, Michael Bay and Peter Jackson, These three directors have spent the most money to make the film.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart7.png" alt="directors with highest revenue" />

<p>Steven Spielberg, Peter Jackson and James Cameron, these three directors have the most revenue by makeing films.

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart8.png" alt="directors with highest B_C" />

<p>Oren Peli who doesn't spent the most money for the production of the film but he made the most profit with the production of the film. Therefore, this director is the most profitable director.</p>
<p>This director was not included in any of the lists of directors with the highest cost and directors with the highest income generation, but still he was the most profitable director.</p>

<h3>Performing statistical operations based on the release date of the film</h3>

<p>First, we make a list of the years in which more than 50 movies were released in that year.
The lowest year is 1994, in which 55 films were released. and the most year is 2016, that year 104 movies were released.
Now we will categorize the films between time periods with a difference of 5 years.
Let's take a look at the number of movies released in these years. The highest number was between 2005-2015 and the lowest number was between 1990-1995.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart9.png" alt="years range number of movies that released" />

<p>The most profitable year is between 2005-2010 and after that it is between 2010-2020.
The least profitable year is between 1990-1995.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart9.png" alt="years range B_C" />

<p>The years 2015-2020 were the most expensive years for film production and 1990-1995 were the least expensive years for film production.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart10.png" alt="years range budget" />

<p>Although the years 2015-2020 were not the most profitable years, they were the most profitable years.
The years 1990-1995 were the least profitable years, but it is estimated to be the most profitable years.
The years 2005-2010 had a relatively low income but a very high profit.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/chart11.png" alt="years range revenue" />
