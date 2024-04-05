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

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/Benefit-Cost-Ratio-Formula.jpg" alt="B_C Formula"></img>

<p>To calculate the benefit per cost obtained from each film made, we have to divide the income by the cost, and if the result is less than one, it means that the film was not profitable, and if the result is more than one, it means that the film was profitable.</p>
<p>We can subtract the results by one and then compare it with zero.</p>
<p>Now we can easly determine which movie is profitable or not profitable.</p>

<h3>How much does it cost to make each genre of film?</h3>
<h3>How much is the benefit of each movie genre?</h3>

<p>By drawing a bar graph, it can be understood that the highest cost is required to make a movie with the action genre, and the lowest cost is required to make a movie with the "tv movie" genre.</p>

<img src="https://github.com/Amin1384Movahedi/TMDB_Movie_Recommendation/blob/main/assets/Budget_per_Genre.png" alt="budget per genre chart"></img>