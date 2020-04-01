# ETL-Project

Extracted, cleaned, and loaded musical data into Postgres to see if there is a correlation between most popular genres of music.


  **Extract: original data sources and how the data was formatted.**
  
	https://data.world/kcmillersean/billboard-hot-100-1958-2017 - import.io
	https://www.kaggle.com/nadintamer/top-spotify-tracks-of-2018 - API


  **Transform: data cleaning and transformation.**

Cleaning: Removed unused columns, Song titles, column names, removing duplicates while maintaining the lowest peak position and the highest amount of weeks on the chart(using a sort function), transposed dates from string to an integer date, dropped songs that did not chart.

Inner joining: On song name to combine song attributes with Billboard position information.

Correlating each list of attributes with peak position and weeks on the Billboard Hot 100. 


  **Load: the final database, tables/collections.**

Relational  - PGAdmin SQL
