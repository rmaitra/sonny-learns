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
This means you will need to write a script that:

1. does an HTTP request to http://theaudl.com/spiders/players/szaccaro and grabs the HTML of the page with ``` import requests ``` package
2. store the html in a variable
3. use ```from bs4 import BeautifulSoup``` to parse the HTML and extract elements
4. parse the HTML into the proposed dictionary above

The packages you will need:

- ```requests``` install with ```$ pip install requests```
- ```BeautifulSoup``` you may have to install this with ```$ pip install beautifulsoup4```

Here is an example script of using the two

```python
# import the packages we will use
from bs4 import BeautifulSoup  
import requests

# this is the link we will scrape
page_link ='https://www.website_to_crawl.com'

# fetch the content from url
page_response = requests.get(page_link, timeout=5)

# parse html
page_content = BeautifulSoup(page_response.content, "html.parser")

# extract all html elements where price is stored
prices = page_content.find_all(class_='main_price')  # find content on the HTML page with classes and ids
# prices has a form:
#[<div class="main_price">Price: $66.68</div>,
# <div class="main_price">Price: $56.68</div>]

# you can also access the main_price class by specifying the tag of the class
prices = page_content.find_all('div', attrs={'class':'main_price'})
```
The script that you write should be modular and flexible though. You should be able to put in any spiders player URL and get back their stats. In order to do that, your script should have this skeleton:

```python
from bs4 import BeautifulSoup  
import requests

def get_html(url):
     # logic for GET HTTP request here

def get_stats_from_html(page_response):
     # logic for parsing HTML and getting stats
     
def format_stats_into_dictionary(stats):
     # logic for converting to dictionary here 

def scrape_stats(url):
     page_response = get_html(url)
     parse_html_stats = get_stats_from_html(page_response)
     stats_dictionary = format_stats_into_dictionary(parse_html_stats)
     
# you should be able to feed any player url and your code will be able to scrape the stats     
scrape_stats("http://theaudl.com/spiders/players/szaccaro")

```

### 2. Add Bootstrap elements to your Index.html file on your website
You have your ```index.html``` for this week. In this assignment you will add bootstrap 4 elements to your app. I think the bootstrap.min.css in your public directory is bootstrap 4, you should double check. If it isn't, please download the bootstrap 4 package from https://getbootstrap.com/ and add the bootstrap.min.css to your public directory. Here are the elements you will add:

1. change the navbar color https://getbootstrap.com/docs/4.0/components/navbar/#color-schemes
2. add a carosoul with image links that you'd like on your site https://getbootstrap.com/docs/4.1/components/carousel/ (NOTE: you need to also make sure that your index.html imports bootstrap.min.js)
3. add an intro to your page in a jumbotron https://getbootstrap.com/docs/4.1/components/jumbotron/
4. add a button that will open a modal https://getbootstrap.com/docs/4.1/components/modal/#modal-components
5. add a table of information https://getbootstrap.com/docs/4.1/content/tables/
