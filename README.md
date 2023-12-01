# NoSQL Challenge: Module 12

## Objective

The goal for this challenge was to manage a NoSQL database of The UK Food Standards Agency's ratings for establishments throughout the United Kingdom and evaluate the information for food critics and journalists to direct their attention on future work. This process involved updating a nosql database using MongoDB, updating the database with information of a new establishment that recently opened, and running exploratory analysis of the database to compile lists that satisfy certain criteria.

### Method
This was done using Python on MongoDB through a Jupyter notebook.

### Exploratory Analysis
First a query was made to compile establishments that had a poor hygiene score of 20, of which 41 results were generated and compiled into a dataframe. Second, a query was made to pull the establishments from London that have a Rating Value of 4 or higher. 33 establishments fit this criteria, and this was compiled into a dataframe. Third, the top 5 establishments with a Rating Value of 5, sorted by the lowest hygiene score was generated, using the location of "Penang Flavours" (which was the newest establishment added to the database). These 5 spots, "Lucky Food & Wine", "Fineway Cash & Carry", "Everest Stores Ltd", "Premier Express", and "TIWA N TIWA African Restaurant Ltd" were compiled into a dataframe for later use. Lastly, a pipeline was created to aggregate the total count of establishments within each Local Authority in the UK that have the lowest possible hygiene score of 0, where the top 10 local authority counts were compiled into a dataframe.

## Attributions

All information sourced and generated in this code is from the course material:<br/>
- Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).
    - https://www.food.gov.uk/'
    - https://ratings.food.gov.uk/open-data/en-GB'
    - https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/
