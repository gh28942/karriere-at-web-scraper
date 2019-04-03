# karriere-at-web-scraper
Uses Python + Selenium to get content from karriere.at and store it in a CSV file (see description of the .py file).

Web scraper that uses Selenium (Python 3) to get information (title, url, type (part/full time), salary per month (estimation), experience level, location, date) from job entries on the website karriere.at using a VPN. Multi threading (three threads) is used to reduce the time the web scraping occupies. The information is then stored in CSV files.

Wage info isn't explicitly stated on the website, so my code uses an algorithm (using e.g. regular expressions) I made to find the salary information in the text. Because of this, it is a value that can only be estimated. If no salary information was found, then the default value zero will be stored in the CSV file.
