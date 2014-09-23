web_spiders
===========

Practice code that incudes:

Spyder
------
- A Scrapy web scraper that finds links from a webpage, and then saves the link data to an Oracle backend.
  - Additionally, Link Spyder saves link data as a local json file (data.json).


Link Spyder Project
-------------------
- Django webserver that reads link data (populated via webscraper) from a local Oracle database.


Link Visualizor
---------------

*In progress*

- An html/javascript Visualion of the scraped data contained in data.json (saved by Spyder - above). 
  - This inplementation uses (D9) CodeFlower.js: http://redotheweb.com/CodeFlower/
  
- Example:
     This json file is visualized as the screenshot below. The centre node represents the url that was scraped,    http://www.dal.ca/dept/its.html. The surrounding nodes represent the links scraped. Hovering the mouse pointer over a will produce a popup displying the link "name". The size attribute is an abutrary weight used in this case to draw a node to the screen.
  
{"size": "20", "name": "http://www.dal.ca/dept/its.html",
    "children": [{"name": "About", "size": "50"},
                 {"name": "Admissions", "size": "50"},
                 {"name": "Academics", "size": "50"},
                 . . .
                 
                 {"name": "Contact Us", "size": "50"}, {"name": "Current Students", "size": "50"},
                 {"name": "Faculty & Staff", "size": "50"}]}


  ![link_nodes](https://cloud.githubusercontent.com/assets/2049888/4366866/9bc95cd0-42c7-11e4-88a3-e272e4d5335a.png)




