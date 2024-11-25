# 2024-DataManagement-Project

Data Management Project for year 2024
Exploring the relationship between pollution and weather conditions: an European analysis



Overview:

This project focuses on data management using MongoDB and Python. It is a data management code that enables import, transformation, and a little analysis using MongoDB as the primary database and Python as the programming language. The code is used to develop a brief analysis about pollution measurements and weather condition of following European States with observations related to the entire year 2022:
• Italy (IT)
• Switzerland (CH)
• Spain (ES)
• France (FR)
• Belgium (BE)
• Netherlands (NL)
• Germany (DE)
• Portugal (PT)
• Great Britain (GB)
• Ireland (IE)
• Austria (AT)
• Norway (NO)
• Finland (FI)
• Sweden (SE)

In particular we have structured our analysis on the following research questions:
• What are the European average O3 levels across maximum temperature ranges?
• What are the European average NO2 levels across precipitation ranges?
• What are the European average PM10 levels across different wind speed ranges?
• What are the European average values of PM10 by season?
• How do pollution measures vary over time in Italy?
• What are the 5 records with the highest PM2.5 values observed in Italy? Where were these values ob-
served? What were the meteorological conditions on those days?

The code is developed in a Jupyter notebook, divided in sections and adequately commented, in order to facilitate the understanding and reproducibility.



Features:

 * Data Acquisition: Download data through 2 API:
    _Pollution: https://openaq.org. It's a closed API and it requires an API key, username and password. The documentation can be seen, along with the list of endpoints here: https://docs.openaq.org/reference/introduction-1 
    _Weather: https://open-meteo.com/. It's an open API and the documentation and the list of endpoints can be seen here: https://open-meteo.com/en/docs/

After the download we have stored the data using MongoDB Atlas, as raw data.
    
 * Data Profiling: Analysis of consistency and completeness of the 2 collections (pollution and weather) in order to assess data quality and develop a good strategy of cleansing. 
    
 * Data Integration and Cleansing: Performing of transformation operations on the data stored in MongoDB to prepare it for analysis. In particular, the 2 collections are integrated, cleaned and are transformed with well-defined structure.
    
 * Data Enrichment: Adding of new feature in order to improve the meaning of the data with description of weather condition and other aspects.
    
 * Data Analysis: Utilized Python to make queries and plot the results with MongoDB charts feature.



Requirements:

In order to reproduce the project, install and utilize the following items: 
    MongoDB Atlas: Utilize cloud MongoDB (https://cloud.mongodb.com) to store the data. Create an account, handle the users permissions and, then, create the db and its collections to store the data. We have chosen it in order to work together in remote and because the documents are structured in a BSON format, a schema that facilitates the integration of the data at a later stage as the fields can themselves have sub-document. 
    Python and Jupyter Notebook: Must be installed along with the necessary libraries such as pymongo, pandas, matplotlib, numpy, bson, seaborn and certifi to handle every aspect of manipulating the data.



Usage:

The code can be run following the order of the sections.
To simply see the final query based on our data exclusively the sections "Libraries", "Connection to MongoDB" and "Query" have to be run.


