## Part 2 Assignments

### 1. Python Web Scraper
You are going to create a python script that scrapes a web pages HTML, then grabs specific data on the page and stores the data in a python dictionary. This goes over:

- HTTP requests
- HTML manipulation
- string manipulation
- python dictionaries (or objects)
- JSON formatting

Specifically you will write a python script that will scrap all the player stats from the AUDL spiders:

http://theaudl.com/spiders/players/szaccaro

Your goal is to scrape the player page, and gather all regular season data and place into a python dictionary that will look like so:
```python
{
   "2018":{
        "games":7,
        "points_played":192,
        "team":"SJ",
        "assists":25,
        "goals":10,
        "blocks":4,
        "plus_minus":21,
        "completions":372,
        "completion_percentage":95.60,
        "hockey_assists":23,
        "turnovers":INFINITY
   },
   "2017":{
        # etc...
   } # and so on
}
```

```python
from bs4 import BeautifulSoup
import requests
page_link ='https://www.website_to_crawl.com'
# fetch the content from url
page_response = requests.get(page_link, timeout=5)
# parse html
page_content = BeautifulSoup(page_response.content, "html.parser")

# extract all html elements where price is stored
prices = page_content.find_all(class_='main_price')
# prices has a form:
#[<div class="main_price">Price: $66.68</div>,
# <div class="main_price">Price: $56.68</div>]

# you can also access the main_price class by specifying the tag of the class
prices = page_content.find_all('div', attrs={'class':'main_price'})
```
