
1.Topic OF ANALYSIS:
Investigating TMDb Movie Database..



2.ABOUT THE DATASET:
The data set contains information about 10,000 movies collected from The Movie Database (TMDb), including user ratings and revenue.
Certain columns, like ‘cast’ and ‘genres’, contains multiple values separated by pipe (|) characters.
The final two columns ending with “_adj” show the budget and revenue of the associated movie in terms of 2010 dollars, accounting for inflation over time.



3.INTRO TO PROJECT:
In this project, I analyzed the TMDb dataset and then communicated my findings about it. I used Jupyter notebook for the complete project. The libraries used were Python libraries - NumPy, pandas,csv and Matplotlib,sns which made my analysis quite easier.


4.DATA WRANGLING:
Data  Wrangling was the key step as many rows contained Null values. Only one duplicate was found. Apart from this many values for budget_adj and revenue_adj were 0, these were also removed to prevent outliers and to prevent calculation of wrong profit. Undesired columns were removed. Also some columns were converted to desired datatype.
After data wrangling, around 3848 movies were the ones which appeared to have correct data for analysis.




5.QUESTIONS ANALYSED:

A. General Statistics..(count, max, min, mean, quartiles etc)

B. What are the movies with max and min
-Popularity
-Revenue
-Budget
-Runtime
-Profit

C. What is the average runtime of all movies?

D. What are the top 10 movies by vote average (Average rating) and popularity?
 
E. Finding top 10 count for:
-Which directors directed max no movies
-Which cast appeared most
-Which genre occured most?

F. What are the characteristics of most profitable movies...?

G. In which year, month we had the most movies making max profits?
-Which month released max,min no of movies overall?
-Which month had sum of profit for all movies max,min?
-Which year released max,min no of movies overall?
-Which year had sum of profit for all movies max,min?

H. Relationship between Various parameters..





6.ANALYSIS AND CONCLUSIONS:

a. Out of given dataset only `3848` movies contained valid data.

b. `Jurassic World` is the movie with max popularity of almost 33.

c. `Avatar movie` has made most revenue.. Making a revenue of more than $2.8B

d. `Star Wars` film has the highest profit in all, making over $2.7B

e. `Average runtime` of all movies is approx 109 min.

f.  The top rated movies are `The Shawshank Redemption` and `Stop Making Sense` with a rating of 8.4.

g.  The directors with max number of  movie releases( more than 20) are:
 - `Steven Spielberg` with 27 movies
 - Clint Eastwood with 24 movies
 - Ridley Scott with 21 movies

h. The cast members which appeared in most movies are:
 - `Robert De Niro`  with   52 movies
 - Bruce Willis      with   46 movies
 - Samuel L. Jackson with   44 movies
 - Nicolas Cage      with   43 movies
 
i. Most filmed genre movies: 
 - `Drama`            1752
 - Comedy             1357
 - Thriller           1202
 - Action             1084
 
j. The characteristics of most profitable movies($10 Million):
 - Directors 	  - Steven Spielberg, Clint Eastwood, Tim Burton, Ridley Scott, Robert Zemeckis
 - Cast      	  - Tom Cruise, Tom Hanks, Brad Pitt, Robert De Niro, Bruce Willis  
 - Genre          - Drama, Comedy, Thriller, Action, Adventure
 - Release months - May, June, July, November, December.
 - Budget Range   - `$224 to $368371256`



7.LIMITATIONS of the dataset and analysis:

a. Unnecessory columns needed to be removed such as imdb_id, budget, revenue, homepage, keywords, overview, production_companies, tagline. This was done because either these contained large no. of null values or didn't seem promising enough to be fit for some analysis.

b. We have not considered type of vote - positive or negative or any other value.

c. Also this dataset had one duplicate row. We had to remove that duplicate row for setting one column(here id) as the index of whole dataset.

d. Due to wrangling lot of movie data needed to be removed, so our analysis is limited to partial no. of movies. ( Only those movies were considered, whose data was valid and without any null values...)

e. There were lot of movies where the budget_adj or revenue_adj have a value of '0' which means that the values of those variables had not been recorded. Calculating the profits of these movies would lead to inappropriate results. So we needed to delete those rows.

f. Dropping missing or Null values from variables of our interest might skew our analysis and could show unintentional bias towards relationship being analyzed.

g. There is no normalization or exchanges rate or currency conversion is considered during this analysis and our analysis is limited to the numerical values of revenue, budget etc.


WHAT DID I LEARN:
The project helped me learn a lot about data analysis, data wrangling techniques, use of various python libraries for analyis..
After completing the project, I :

- now know all the steps involved in a typical data analysis process.
- am comfortable posing questions that can be answered with a given dataset and then answering those questions.
- know how to investigate problems in a dataset and wrangle the data into a format that can be used.
- have practice of communicating the results of the analysis.
- am able to use vectorized operations in NumPy and Pandas to speed up your data analysis code.
- familiar with Pandas Series and DataFrame objects, which lets access data more conveniently.
- lastly but not least, I know how to use Matplotlib and Seaborn to produce plots showing findings.



REFERENCES:
Some references made during the project are as follows:

1. stackoverflow.com
2. analyticsvidhya.com
3. python documentation(for datetime, matplotlib, seaborn and csv)
4. matplotlib.org
5. seaborn.pydata.org


