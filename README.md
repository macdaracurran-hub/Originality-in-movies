# Originality-in-movies
A personal project completed with another UCD student, Nathan Mahady to examine the originality, or lack theroff of modern cinema. 

Notes on data collection IMDB
For the data collection there are two folders IMDb_DataCollection and TMDb_DataCollection.
In IMDB_Data collection the contents are the following.
All notebooks with scraping in the title are used to webscrape IMDB, for oneoff movies, remakes and sequels.
All files with output at the end of them were scraped from IMDB, Sequel Output is the output of sequel scraping etc.
Standalone Output was taken from oneoff scraping.ipynb because we were using different terminology at the time
refering to oneoffs as standalone movies.
All other files in this folder contain IMDb Id's which are used to run the webscraper notebooks.
#Notes on research questions
For the research questions, RQ1, RQ2, RQ3 and RQ4 can all be run using the files inside the folder.
#Notes on enviroment
We did not set up an enviroment, but you should be able to run our code as long as you have the latest version of matplotlib
If you need to update it you can use, pip install --upgrade matplotlib   , to upgrade matplotlib
There is also a package named prettytable used to once or twice, you may not have this.
If you need to install it you can use, pip install prettytable   , to install prettytable.

List of Main files and Notebooks used. Taken from Final report.
#Datasets
Datasets Used


remakes_data.csv - Main data set used in all research questions containing the data about
remakes and the original movies for those remakes.


sequels_data.csv - Main data set for research questions 1 and 2. Contains the data about
sequels and the original movies for those sequels.


sequels_edit.csv - Main data set for research questions 3 and 4. Contains the data about
sequels and the original movies for those sequels. Very similar to sequels_data, but with
further data cleaning done to get more accurate revenue figures.


StandAloneIMDb.csv - Dataset that was used in research questions 2 & 4. Has information
from IMDB about standalone / one-off movies.


StandAloneTMDb.csv - Data set that was used in research questions 2 & 4. Has information
from TMDB about standalone / one-off movies


#Notebooks


OneoffScraping.ipynb – Scraping notebook that uses original_movies.csv to web scrape
movie data from IMDB. Produces StandAloneIMDb.csv.


RemakeScraping.ipynb – Scraping notebook that uses remade_imdbs.csv to web scrape
movie data from IMDB. Produces RemadeOutput .csv.


SequelsScraping.ipynb – Scraping notebook that uses movies_data.csv to web scrape movie
data from IMDB. Produces SequelsOutput.csv.


1000_data_gathering_standalones.ipynb - Uses movie_ids_01_01_2023.json.gz (TMDB
data dump) and gathers data for standalone movies from TMDB to produce original_movies.csv


1100_data_cleaning_standalones.ipynb - Merges NewOriginal.csv and standalones_tmdb_data.csv
and cleans data to produce standalones_data.csv.


1200_data_gathering_remakes.ipynb - Uses RemadeOutput.csv and gathers data from
TMDB for remakes to produce remakes_tmdb_data.csv.


1300_data_cleaning_remakes.ipynb - Merges RemadeOutput.csv and remakes_tmdb_data.csv
and cleans data to produce remakes_data.csv.


1400_data_gathering_sequels.ipynb - Uses SequelIMDBlinks.csv and gathers data from
TMDB for remakes to produce sequels_tmdb_data.csv.


1500_data_cleaning_sequels.ipynb - Merges SequelOutput.csv and sequels_tmdb_data.csv
and cleans data to produce sequels_data.csv.


RQ1.ipynb - Notebook used to answer research question 1


RQ2.ipynb - Notebook used to answer research question 2


RQ3.ipynb - Notebook used to answer research question 3


RQ4.ipynb - Notebook used to answer research question 4
