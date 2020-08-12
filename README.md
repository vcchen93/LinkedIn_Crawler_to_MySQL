# LinkedIn_Crawler_to_MySQL
The is a demostration of crawling information from LinkedIn and store them into MySQL
The crawler use [Selenium](https://github.com/SeleniumHQ/selenium)(chrome version) to get data from LinkedIn.

### Requirements
The following file is needed. Please download and put it in the same folder as the crawlers.
* [chromedriver](https://chromedriver.chromium.org/) Please get a chromedriver that matches your version of chrome. This is required by Selenium to run LinkedIn crawler.

### MySQL Setting
For the crawler, 1 MySQL schema and 2 tables will be needed.
* Schema Nmae: linkedin
* Table 1: lk_urls:
columns=['id'(AI),'urls'(UI),'keywords']
* Table 2: lk_data:
columns=['id'(PK),'Name','Location','About',\
             'Position_1','Company_1','Dates_Employed_1', 'Time_Employed_1', 'Location_Employed_1', 'Job_Description_1',\
             'Position_2','Company_2','Dates_Employed_2', 'Time_Employed_2', 'Location_Employed_2', 'Job_Description_2',\
             'Position_3','Company_3','Dates_Employed_3', 'Time_Employed_3', 'Location_Employed_3', 'Job_Description_3',\
             'School_Name_1', 'Degree_Name_1', 'Degree_Time_1', 'Degree_Description_1', \
             'School_Name_2', 'Degree_Name_2', 'Degree_Time_2', 'Degree_Description_2', \
             'School_Name_3', 'Degree_Name_3', 'Degree_Time_3', 'Degree_Description_3', \
             'Certification_Name_1', 'Certification_Auth_1',\
             'Certification_Name_2', 'Certification_Auth_2',\
             'Certification_Name_3', 'Certification_Auth_3',\
             'Skill_1', 'Skill_2', 'Skill_3', 'urls'(UI)]

### Usage
* LinkedIn_Crawler_get_urls.ipynb:
  Search for profile urls from LinkedIn with a given keyword.
* LinkedIn_Crawler_get_data.ipynb:
  Receive ids and urls from MySQL and crawl profile information.
