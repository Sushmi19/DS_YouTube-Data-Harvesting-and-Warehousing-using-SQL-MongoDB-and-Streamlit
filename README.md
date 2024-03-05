YouTube-Data-Harvesting-and-Warehousing-using-SQL-MongoDB-and-Streamlit.

Problem Statement: 
The problem statement is to create a Streamlit application that allows users to access and analyze data from multiple YouTube channels.

Introduction:

This project is a YouTube API scrapper that allows users to retrieve and analyze data from YouTube channels. It utilizes the YouTube Data API to fetch information such as channel statistics, video details, comments, and more. The scrapper provides various functionalities to extract and process YouTube data for further analysis and insights.

Features:
The YouTube Data Scraper offers a range of features to help you extract and analyze data from YouTube. Some of the key features include:

Retrieve channel statistics: Get detailed information about YouTube channels, including subscriber count, view count, video count, and other relevant metrics.

Fetch video details: Extract data such as video title, description, duration, view count, like count, dislike count, and publish date for individual videos.

Analyze comments: Retrieve comments made on YouTube videos and perform analysis, such as sentiment analysis or comment sentiment distribution.

Generate reports: Generate reports and visualizations based on the collected data, allowing users to gain insights into channel performance, video engagement, and audience interaction.

Data storage: Store the collected YouTube data in a database for easy retrieval and future reference.

1. Tools Install:

Virtual code.
Jupyter notebook.
Python 3.11.0 or higher.
MySQL.
MongoDB.
Youtube API key.

2. Requirement Libraries to Install:

pip install google-api-python-client, pymongo, mysql-connector-python, sqlalchemy, pymysql, pymysql, pandas, numpy, plotly-express, streamlit.
( pip install google-api-python-client pymongo mysql-connector-python sqlalchemy pymysql pandas numpy plotly-express streamlit )

3. Import Libraries:
   
Youtube API libraries

import googleapiclient.discovery
from googleapiclient.discovery import build
File handling libraries

import json
import re
MongoDB

import pymongo
SQL libraries

import mysql.connector
import sqlalchemy
from sqlalchemy import create_engine
import pymysql
pandas, numpy

import pandas as pd
import numpy as np
Dashboard libraries

import streamlit as st
import plotly.express as px

4. E T L Process:
   
a) Extract data
Extract the particular youtube channel data by using the youtube channel id, with the help of the youtube API developer console.
b) Process and Transform the data
After the extraction process, takes the required details from the extraction data and transform it into JSON format.
c) Load data
After the transformation process, the JSON format data is stored in the MongoDB database, also It has the option to migrate the data to MySQL database from the MongoDB database.

5. E D A Process and Framework:
   
a) Access MySQL DB
Create a connection to the MySQL server and access the specified MySQL DataBase by using pymysql library and access tables.
b) Filter the data
Filter and process the collected data from the tables depending on the given requirements by using SQL queries and transform the processed data into a DataFrame format.
c) Visualization
Finally, create a Dashboard by using Streamlit and give dropdown options on the Dashboard to the user and select a question from that menu to analyse the data and show the output in Dataframe Table and Bar chart.

User Guide:

Step 1. Data collection zone
Search channel_id, copy and paste on the input box and click the Get data and stored button in the Data collection zone.
Step 2. Data Migrate zone
Select the channel name and click the Migrate to MySQL button to migrate the specific channel data to the MySQL database from MongoDB in the Data Migrate zone.
Step 3. Channel Data Analysis zone
Select a Question from the dropdown option you can get the results in Dataframe format or bar chat format.

