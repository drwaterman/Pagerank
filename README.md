# Pagerank
This application is a simple model of a search engine written in Python and using an SQLite database. 

* **spider.py** crawls a given website, loads the pages into the database, and records the links to other pages.

* **spdump.py** prints the database to the console

* **sprank.py** takes the database created by spider.py and gives each page a rating based on how many other pages link to it.

* **spreset.py** resets the rankings to 1.0, so that the rankings can be recalculated without downloading all of the pages again.

* **spjson.py** creates spider.js JSON output from the page rankings.

* **force.html** loads spider.js and creates a force-directed graph based on the page rankings using the d3 library from http://mbostock.github.com/d3

The data currently stored in the database and displayed at force.html comes from crawling the jmu.edu website.
