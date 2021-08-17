# Surfs-UP Business Analysis with SQLAlchemy and Flask

SQLAlchemy (source code) is a Python library for accessing persistent data stored in relational databases either through raw SQL or an object-relational mapper. Sqlite is a database storage engine, which can be better compared with things such as MySQL, PostgreSQL, Oracle, MSSQL, etc. It is used to store and retrieve structured data from files. We will be using SqlAlchemy to access and retrieve information from Sqlite. 

Flask is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. Below are the advantages:

* Higher compatibility with latest technologies.
* Technical experimentation.
* Easy to build a quick prototype.
* Routing URL is easy.
* Easy to develop and maintain applications.

## Overview of Project

During a vacation to Oahu, we are planning to open a Surf & Shake shop there and settle. So we planned to meet the Investor W. Avy. But before the meet up we have to work on Projected Revenue Vs Expenses & Investment Breakdown. For this we need to work on the Sqlite database and extract the weather summary as its a important factor for surfing. As of now we are mainly interested to find the below details:

  *	The Summary Statistics for June
  *	The Summary Statistics for December
  *	Key differences between June and December weather
  *	Additional queries to perform to gather more weather data
   
## Analysis 

Before we start doing our Analysis, we need to setup the dependencies for SqlAlchemy and basic engine & session setup to connect the Sqlite Database "hawaii.sqlite". Below are the dependencies we need:

![image](https://user-images.githubusercontent.com/85472349/129511939-ddec48d7-86d5-4c28-a5df-d5d68e2897ce.png)
  
### The Summary Statistics for June

In this we are using Python, Pandas, and SQLAlchemy to do the below steps to generate the summary statistics for June:

* Filter the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for the month of June.

![image](https://user-images.githubusercontent.com/85472349/129512394-3fa04a67-1686-4d3b-b3a0-386663dbf8d7.png)

* Converting those temperatures to a list 

![image](https://user-images.githubusercontent.com/85472349/129512416-90c2932e-0a3b-4ab0-a257-45647a312558.png)

* Also create a DataFrame from the list and the DataFrame is displayed 

![image](https://user-images.githubusercontent.com/85472349/129512451-693c5893-3926-4191-a6e9-e1f76e1824fc.png)
 
* The summary statistics is generated for the month of June.

![image](https://user-images.githubusercontent.com/85472349/129512473-6084a1bf-e0a7-4ae3-80b8-6b4bee72ca4c.png)

### The Summary Statistics for December

In this we are using Python, Pandas, and SQLAlchemy to do the below steps to generate the summary statistics for December:

* Filter the date column of the Measurements table in the hawaii.sqlite database to retrieve all the temperatures for the month of December.

![image](https://user-images.githubusercontent.com/85472349/129513407-154a0a48-b917-4386-8320-6a34ccce4c34.png)

* Converting those temperatures to a list 

![image](https://user-images.githubusercontent.com/85472349/129513435-11274225-8cf7-4499-a0d0-6a6d851e7d4f.png)

* Also create a DataFrame from the list and the DataFrame is displayed 

![image](https://user-images.githubusercontent.com/85472349/129513462-51de0b54-ed77-4a39-b8d4-32a333d2f230.png)
 
* The summary statistics is generated for the month of December.

![image](https://user-images.githubusercontent.com/85472349/129513487-a54c3d51-0fa0-41c8-ae12-d4403a113288.png)


## Results

Here are the links for python and sqlite files:

1) 

2) 


#### Key differences between June and December weather

We have got the summary Statistics for the month of June and December. So now its time for comparison to get some conclusion. 

1) The number of counts, and all the other statistic values are little bit higher in the month of June.

![image](https://user-images.githubusercontent.com/85472349/129514695-c0d2318f-f212-4d59-ac40-a53f68d127ab.png)

2) Difference between Mean and statistic quartile values are 3 or 4 points differ in both months.

![image](https://user-images.githubusercontent.com/85472349/129514834-9036e373-fecc-42b6-bd5b-ed0931ab4a86.png)

3) The Minimum temperature is little lower in December and Maximum temperature is little higher in June as we expect in Summer & winter. But we have to note that its not too cold in December, which means surfing is possible in winter too.  

![image](https://user-images.githubusercontent.com/85472349/129514923-500408a5-2eb3-43f1-a026-d594b5d98e8d.png)


## Summary

We can even perform some more analysis for better understanding and profitable business: 

#### 1) Values per Station 

We can find the counts for each station and statistical values for station with highest count:

* Below are the results for June month:

![image](https://user-images.githubusercontent.com/85472349/129515438-8842e513-19fb-45a9-b896-28cef0836cdd.png)

* Below are the results for December month:

![image](https://user-images.githubusercontent.com/85472349/129515521-d62243d0-f1cf-424f-9541-66c4e669446c.png)


#### 2) Plot with bins 

The plot with bin values will give a look-good feel of the data. Below are the plots for June & December month:

![image](https://user-images.githubusercontent.com/85472349/129515702-7d96ec13-e07c-43ae-bb6a-88b83b88b40b.png)



**Hurry! Surf & Shake Shop is ready to open in Oahu !!!**