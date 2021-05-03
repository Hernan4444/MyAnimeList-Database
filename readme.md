# MyAnimeList Database 2020

This dataset contains information about 17.562 anime and the preference from 325.772 different users. In particular, this dataset contain:

- The anime list per user. Include dropped, complete, plan to watch, currently watching and on hold.
- Ratings given by users to the animes that they has watched completely.
- Information about the anime like genre, stats, studio, etc.
- HTML with anime information to do data scrapping. These files contain information such as reviews, synopsis, information about the staff, anime statistics, genre, etc.

Also, the dataset is available at kaggle: https://www.kaggle.com/hernan4444/anime-recommendation-database-2020

### Warning: this dataset includes information about anime for adults (hentai). 


## Content

* The "html" folder contain 1 zip per anime (17.562 different anime). Each zip contains different HTML pages scrapped from [MyAnimeList](https://myanimelist.net/).

* `animelist.csv` have the list of all animes register by the user with the respective score, watching status and numbers of episodes watched. This dataset contains 109 Million row, 17.562 different animes and 325.772 different users.

* `rating_complete.csv` is a subset of `animelist.csv`. This dataset only considers animes that the user has watched completely (`watching_status==2`) and gave it a score (`score!=0`). This dataset contains 57 Million ratings applied to 16.872 animes by 310.059 users.

* `anime.csv` contain general information of every anime (17.562 different anime) like genre, stats, studio, etc.

* `anime_with_synopsis` contain the synopsis of all anime that not include Hentai in Genres.


Each dataset and description is in the [data folder](https://github.com/Hernan4444/MyAnimelist-Database/tree/master/data).


## Acknowledgements

Thanks to:
1. [MyAnimeList](https://myanimelist.net/) for providing anime data.
2. [Jikan API](https://jikan.docs.apiary.io/) for provide users preference.
3. Pontificia Universidad Católica de Chile for provide servers to run the code.


## Inspiration

1. Have an HTML files to experience the scraping exercise without the delay of each requests.

2. Experiment with different types of recommended. For instance, collaborative filtering or based on context like stats, genre, seiyus, reviews, synopsis, etc.

3. Use this information to build a better anime recommended system.

4. Identifying which feature allows us to build the best anime recommended system.


## Ideas to the future

1. Build the same dataset with manga and novel.
