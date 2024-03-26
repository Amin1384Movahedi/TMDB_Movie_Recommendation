# TMDB_Movie_Recommendation

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
Copy code
<p>
   <strong>Note:</strong> This README.md file is a HTML conversion of the original markdown file. Some formatting may be lost in the conversion process.
</p>
<p>
   <strong>Additionally:</strong> This README.md file includes a table of contents for easy navigation.
</p>
<h2>Table of Contents</h2>
<ul>
   <li><a href="#background">Background</a></li>
   <li><a href="#data-source-transfer-summary">Data Source Transfer Summary</a></li>
   <ul>
      <li><a href="#good-news">Good News</a></li>
      <li><a href="#bad-news">Bad News</a></li>
      <ul>
         <li><a href="#bad-entries">Bad Entries</a></li>
      </ul>
   </ul>
</ul>
Copy code
<p>
   Note: This is a simple HTML conversion of the original markdown file. Some formatting may be lost in the conversion process.
</p>
<p>
   Additionally: This HTML file includes a table of contents for easy navigation.
</p>
<p> <strong>References:</strong> </p>
<ul>
   <li> <a href="https://www.kaggle.com/tmdb/tmdb-movie-dataset" target="_blank">TMDb Movie Dataset</a> </li>
   <li> <a href="https://www.themoviedb.org/documentation/api" target="_blank">The Movie Database API</a> </li>
   <li> <a href="https://www.imdb.com/interfaces/" target="_blank">IMDb Interface</a> </li>
</ul>
<p> <strong>License:</strong> </p>
<p> The contents of this repository are covered under the <a href="https://github.com/Kaggle/tmdb-movies/blob/master
