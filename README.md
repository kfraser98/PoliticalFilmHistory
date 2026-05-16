## Title: 
Mirrors or Coincidences

## Description:
Since the war propaganda films of the 1940s, film has been used to both mirror and shape political consciousness in the United States. This project explores whether that relationship is still relevant today during one of the most politically turbulent decades in modern history.
Three groups of films were examined: the top 10 highest-grossing domestic films per year, award-nominated films from the Academy Awards and Golden Globes, and highly-rated films from TMDb. A political and social event timeline from 2016-2025 was created to provide context. 

## Workflow:
* Extract top 10 highest rated films with genre IDs from 2015-2025 using the TMDb API and export it as a CSV, use search and replace in Excel to convert genre ID numbers into words.
* Extract top 10 highest grossing films from 2015-2025 using the unofficial BoxOffice Mojo API and export it as a CSV file.
* Create a file of Academy Award nominees and winners from the 2016-2026 ceremonies from major categories (including but not limited to Best Picture, Best Actor/Actress, Best Screenplay - Original/Adapted) and convert to CSV.
* Download Golden Globes dataset from Kaggle and extract nominees and winners in major categories (including but not limited to Best Picture - Drama/Comedy, Best Actor/Actress, Best Screenplay) from the years 2016-2020, supplement 2021-2026 data from the Golden Globes website in Excel and convert to CSV.
* Combine the Golden Globes and Academy Award data in Open Refine.
* Extract the films with the most nominations and most wins in python. Save file as csv.
* Determine statistical relationship between awards nominations and TMDb rating and box office revenue using scipy.stats, numpy, and pandas libraries.
* Compile political events timeline using headlines and articles from major news sources (CNN, NBS, PBS, NPR)
* Pick overlapping films between awards x box office and awards x rating, along with other films with the most wins (10 total) for further thematic analysis.
* Analyze film themes based on IMDb plot synopsis and previous watches.
* Compare themes with the political events timeline.

Tools Used:
* TMDb API
* Unofficial BoxOffice Mojo API
* Academy Awards database
* Kaggle dataset (for Golden Globes data)
* 'pandas' python library
* 'scipy' python library
* 'numpy' python library
* OpenRefine
* Excel

## Further Uses:
This project can be expanded to further map a relationship between popular film and political events. All datasets can be expanded to include previous and future years to get a better understanding of which films become popular either critcally or culturally. The amount of films chosen for thematical analysis can grow as well. Additionally, this project can be expanded to look at genre trends to see if certain genres become more or less popular during certain times.

## Files List:
* 2026-04-24_academy_awards2016-2026.csv - Academy Awards Data
* 2026-04-24_goldenglobes2015_202.csv - Golden Globes Data
* 2026-04-28_most_nominated.csv - Most Nominated Films from Academy Awards and Golden Globes
* 2026-04-28_tmdb_data.ipynb - Python Notebook to extract TMDb data
* 2026-05-08_boxoffice_data.ipynb - Python Notebook to extract Box Office Mojo data
* 2026-05-08_film_awards_summary.csv - Summary of Academy Awards and Golden Globes data
* 2026-05-09_chisquare_test.ipynb - Python Notebook for chi-square test
* 2026-05-09_film_thematic-analysis.csv - Film Thematic Analysis
* 2026-05-10_political_event_timeline.csv - Political Events Timeline
