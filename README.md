# LinkedIn_Crawler_to_MySQL
The is a demostration of crawling information from LinkedIn and store them into MySQL
The crawler use [Selenium](https://github.com/SeleniumHQ/selenium)(chrome version) to get data from LinkedIn.

### Requirements
The following file is needed. Please download and put it in the same folder as the crawlers.
* [chromedriver](https://chromedriver.chromium.org/) Please get a chromedriver that matches your version of chrome. This is required by Selenium to run LinkedIn crawler.

### MySQL Setting
For the crawler, 1 MySQL schema and 2 tables will be needed.
* Schema Nmae: linkedin
* Table 1: lk_urls
* Table 2: lk_data
