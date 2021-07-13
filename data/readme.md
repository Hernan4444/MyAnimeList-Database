# Files/folder description


## html folder

Folder with 1 zip per anime. In this repo, I upload only 5 zip, but all zip (17.562 files) are in "html.zip": https://drive.google.com/drive/folders/1UhinqGrH2XytkpiD7LlLzMcn7MY2I_gt. The file name corresponds to the MyAnimelist ID of the anime. Each zip contains the HTML pages scrapped from [MyAnimeList](https://myanimelist.net/). The scrapped pages are:

- Main page
- Reviews
- Recommendations
- Stats
- Characters & Staff


## animelist.csv

CSV that contain the anime list per user with the respective score, watching status and numbers of episodes watched by the user. This dataset contains 109 Million row, 17.562 different animes and 325.772 different users. The file have the following columns:

1. user_id:  non identifiable randomly generated user id.
2. anime_id: MyAnemlist ID of the anime. (e.g. 1).
3. score: score between 1 to 10 given by the user. 0 if the user didn't assign a score. (e.g. 10)
4. watching_status: state ID from this anime in the anime list of this user. (e.g. 2)
5. watched_episodes: numbers of episodes watched by the user. (e.g. 24)


In this repo, I upload only the file with 500 lines, but the complete file are in this folder: https://drive.google.com/drive/folders/1UhinqGrH2XytkpiD7LlLzMcn7MY2I_gt.


## watching_status.csv

Description of every possible status of the column: "watching_status" in `animelist.csv`. This file have the following columns:

1. status: ID of the status (e.g 2)
2. description: description of the status (e.g Completed)


## rating_complete.csv

CSV that contains the list of ratings given by the user to animes with `watching_status==2` (complete). This dataset contains 57 Million ratings applied to 16.872 animes by 310.059 users. This file have the following columns:

1. user_id:  non identifiable randomly generated user id.
2. anime_id: - MyAnimelist ID of the anime that this user has rated.
3. rating: rating that this user has assigned.

In this repo, I upload only the file with 500 lines, but the complete file are in this folder: https://drive.google.com/drive/folders/1UhinqGrH2XytkpiD7LlLzMcn7MY2I_gt.


## anime.csv

Information of anime scrapped of main page and stats page. This file have the following columns:

1.  MAL_ID:  MyAnimelist ID of the anime. (e.g. 1) 
2.  Name: full name of the anime. (e.g. Cowboy Bebop) 
3.  Score: average score of the anime given from all users in MyAnimelist database. (e.g. 8.78) 
4.  Genres: comma separated list of genres for this anime. (e.g. Action, Adventure, Comedy, Drama, Sci-Fi, Space) 
5.  English name: full name in english of the anime. (e.g. Cowboy Bebop) 
6.  Japanese name: full name in japanses of the anime. (e.g. カウボーイビバップ) 
7.  Type: TV, movie, OVA, etc. (e.g. TV)
8.  Episodes': number of chapters. (e.g. 26)
9.  Aired: broadcast date. (e.g. Apr 3, 1998 to Apr 24, 1999)
10. Premiered: season premiere. (e.g. Spring 1998)
11. Producers: comma separated list of produducers (e.g. Bandai Visual)
12. Licensors: comma separated list of licensors (e.g. Funimation, Bandai Entertainment)
13. Studios: comma separated list of studios (e.g. Sunrise)
14. Source: Manga, Light novel, Book, etc. (e.g Original)
15. Duration: duration of the anime per episode (e.g 24 min. per ep.)
16. Rating: age rate (e.g. R - 17+ (violence & profanity))
17. Ranked: position based in the score. (e.g 28)
18. Popularity: position based in the the number of users who have added the anime to their list. (e.g 39)
19. Members: number of community members that are in this anime's "group". (e.g. 1251960)
20. Favorites: number of users who have the anime as "favorites". (e.g. 61,971)
21. Watching: number of users who are watching the anime. (e.g. 105808)
22. Completed: number of users who have complete the anime. (e.g. 718161)
23. On-Hold: number of users who have the anime on Hold. (e.g. 71513)
24. Dropped: number of users who have dropped the anime. (e.g. 26678)
25. Plan to Watch': number of users who plan to watch the anime. (e.g. 329800)
26. Score-10': number of users who scored 10. (e.g. 229170)
27. Score-9': number of users who scored 9. (e.g. 182126)
28. Score-8': number of users who scored 8. (e.g. 131625)
29. Score-7': number of users who scored 7. (e.g. 62330)
30. Score-6': number of users who scored 6. (e.g. 20688)
31. Score-5': number of users who scored 5. (e.g. 8904)
32. Score-4': number of users who scored 4. (e.g. 3184)
33. Score-3': number of users who scored 3. (e.g. 1357)
34. Score-2': number of users who scored 2. (e.g. 741)
35. Score-1': number of users who scored 1. (e.g. 1580)


## anime_with_synopsis.csv

Information of anime scrapped of main page that include de Synopsis. This file only contain animes that not include Hentai in Genres column. This file have the following columns:

1.  MAL_ID:  MyAnimelist ID of the anime. (e.g. 1) 
2.  Name: full name of the anime. (e.g. Cowboy Bebop) 
3.  Score: average score of the anime given from all users in MyAnimelist database. (e.g. 8.78) 
4.  Genres: comma separated list of genres for this anime. (e.g. Action, Adventure, Comedy, Drama, Sci-Fi, Space) 
5.  Synopsis: string with the synopsis of the anime.


-------------------------------------------

# Another files generate by the code but not upload to keep the anonymity of users.

## users.csv

List of users with their respective randomly and unique id. This file have the following columns:

1. user_id: non identifiable randomly generated user id.
2. username: name of the user in Myanimelist.

## users_list.txt

List of members of all revised clubs.


## clubs.txt

List of some clubs id available in MyAnimelist.


## \_revised\_clubs.txt

List of club ID that have been revised in the code.


## \_last\_revised\_users.txt

User ID from the last user revised in the code.

