# Stock Financial Data Visualization

## Boot Camp Project III
## University of Toronto SCS - Data Analytics

## Overview
The objective of the project is to create Interactive visual representation of Five US Stock data. A user will be able to interactively view various information about these five company which helps them make informative investment decisions.  
The five selected companies are:
1.	Apple
2.	Microsoft
3.	Google
4.	IBM
5.	Cognizant
6.  Tesla
7.  Facebook
8.  McDonald

## Data Source
-	Our company details will be scrape by yahoo finance
-	Our graph data source will be json format from Alpha Vantage API.
-	Our will be 100 data point for each companies
-	Our data is daily adjusted for each companies
-	Our data API returns daily time series (date, daily open, daily high, daily low, daily close, daily volume, daily adjusted close, and split/dividend events).

URL’s:
-	https://www.alphavantage.co/query?function=TIME_SERIES_DAILY_ADJUSTED&symbol=<sticker>&outputsize=compact&apikey=<api_key> 
-	https://ca.finance.yahoo.com/

### Goals
1.	Extract stock data for five major companies using API
2.	Transform the data using python pandas
3.	Load the data to MySQL DB
4.	HTML Visualization of the data
5.	Using Flask for navigation routes
6.	User will be able to lookup company info details visually

### Specifications
Python, Pandas, MySQL, Json, HTML, JavaScript, Plotly, D3, Leaflet, bsoup, jupyter notebook, splinter (browser), request

### HTML 
●	Leverages JavaScript manipulation of the record 
●	Leverage CSS for the styling
●	Leverage Bootstrap for layout canvas
●	Leverage plotly, leaflet for graphs and heatmaps

### Milestones
I.	Extraction
Extraction of the Data occurred from Alpha Vantage API.  Import the following library modules such as requests, json, pandas, datetime, re (regex).

#### Alpha Vantage API access guidance: 
●	Obtain free API key  
●	Use daily adjusted Json API call

#### Yahoo Finance Data scrape guidance: 
●	Beautiful soup
●	Chrome driver
●	Splinter (browser)

II.	Transformation
The following transformation was completed to the data.
●	Drop Null values

III.	Loading
The loading of the data involves the creation RDS on MySQL from data frame.  A connection engine for data load to MySQL.  The data will be in three tables as follows
Table 1 - Yahoo finance data 
Table 2 - Alpha Vantage data 
