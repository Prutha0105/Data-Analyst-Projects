# Instagram Reach Analysis 

| Contents 											 	   	|
| -------- 											 	   	|
| [Dataset Description](#Dataset-Description)			   	|
| [Questions for Analysis](#Questions-for-Analysis)	   		|
| [Data Wrangling](#Data-Wrangling)					   		|
| [Data Cleaning](#Data-Cleaning)						   	|
| [Exploratory Data Analysis](#Exploratory-Data-Analysis)	|
| [Built with](#Built-with)							   		|

## Dataset Description: 
This PProject has instagram data. Pplease check Dataset file "Instagram data.csv"

## Questions for Analysis:
- Do movies with high popularity achive high revenvue?
- What are the most filmed genres in this whole dataset?
- Is there a correlation between a movie budget and its revenue?

## Data Wrangling:
Our data can be found on `instagram data.csv` file provided on this repository. 

## Data Cleaning:
**Main Observations:**
1. Our dataset consisted of a total of 10866 rows and 21 columns.
2. We had only 1 duplicated row which had been dropped.
3. Some columns wont be useful in answering our questions so they were dropped.
4. Few columns had many missing values that needed to be handled.
5. Columns `cast` `director` `genre` had values saperated with a '|'.
6. `release_date`'s data type needed to be casted.
7. We could append a column for the movie `profit` using the formula: $profit = revenue - budget$.
8. `vote_average` better be presented as a catecorical variable that groubs multible ratings values.
9. We might also catigorize `profit` column for better EDA

## Exploratory Data Analysis:
After finishing our dataset cleaning, we endded up with a total of 10840 records and 10 columns. The dataset now has no duplicates nor null values, and the data types are consistant with suitable categorical variable to address our questions.
We then perfomed some analytics and created some visualizations to answer our targeted questions.
### Q1: Do movies with high popularity achive high revenvue?
> More popular movies recieve way more revenue than the less popular movies.

### Q2: What are the most filmed genres in this whole dataset?
> - `Drama`, `Comedy` and `Action` are the most three filmed genres in total of 10839 movies in our dataset.
> - `Drama` genre alone is filmed 22.6% of the times on our dataset.

### Q3: Is there a correlation between a movie budget and its revenue?
> There is positive correlation between `budget` and `revenue`, indecating a relation between them with little outliers found. 

## Built with:
- JupyterLab
- Python3
- Pandas
- Numpy
