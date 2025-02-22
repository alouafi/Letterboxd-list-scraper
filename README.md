# Letterboxd-list-scraper

A tool for scraping Letterboxd lists from a simple URL. The output is a CSV file with film titles, release year, director, cast, rating (only available for personal film lists), average rating and a whole lot more. The current version is tested on watchlists and normal lists. The current scrape rate is about 1.3 seconds per film.

## Getting Started

### Dependencies

Requires python 3.x, numpy, BeautifulSoup (bs4), requests and tqdm. If other dependencies are not met you can install everything needed using `pip install -r requirements.txt` (ideally in a clean virtual environment).

### Installing

* Copy over the repository and work in there.

### Executing program

* Run the program by running `python main.py` and inputting a valid URL (e.g. https://letterboxd.com/bjornbork/list/het-huis-anubis/). After some time a CSV file will be outputted containing your data. See `imdb-top-250.csv` for a preview.
* (Optional) Use the script `cast_reader.py` to read-in the 'Cast' column from the CSV files to proper python lists.

## TO-DO

* Add option such that only particular pages of very long lists can be scraped (e.g. only the first 10).
* Add options for output (CSV, json, txt).
* Add feature that scrapes how many times a movie has been given a specific rating.
* Add more user-specific features (top 4, diary, watched, etc.)?
  
## Authors

Arno Lafontaine  

## Acknowledgments

Thanks to BBotml for the inspiration for this project https://github.com/BBottoml/Letterboxd-friend-ranker.
