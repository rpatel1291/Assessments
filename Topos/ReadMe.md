# Company - Topos
## Position - Data Engineering Summer Internship


## Task Overview

The goal of this assignment is to demonstrate your ability to capture unconventional datasets, clean and store them.

Write a scraper in either python or NodeJS to collect data from Wikipedia about the top cities in the United States. The fields you collect, as well as the volume of data is up to you, but ideally you add additional data beyond the initial table, such as data found on the individual city pages, or other sources of your choice. The final format should be a CSV file that is ready to be uploaded to a BigQuery table. Please read Bigquery’s Manual to prepare your CSV in the right format. Intermediary steps, environments or processes necessary to run the scraper should be documented in code as well as a Readme.md and hosted on github in a repo devoted to this assignment. 


## My Approach

Using Python and Jupyter Notebook to complete the assessment, it made it easier breakdown the process and easier to check output without rerunning the entire Python code. What I did first was import all the common libraries and modules needed such as Selenium, Requests, and BeautifulSoup. The next step was to create a webdriver to get the Top Cities Wiki page and find where the important information is and extract it. The main information I extracted was the table that list all the cities and the information associated with it. However, the time consuming part was each row did not follow a pattern so there needed to be a if-elif-else step to point to the right element. Once completed. I filtered the entire table to the top ten cities and went to their wiki pages to extract the overview, geography, and climate of the cities. Not knowing how much data is needed I stopped here just to show I was able to go through html structures to find information and being able to extact it and store it in a Data Frame. Once the data frame was created, I saved it as a CSV file and imported to a BigQuery Table.