# An Analysis of Restaurant Turnover in Vancouver


## Overview

Vancouver is famous for being a city with a great diverse selection of cuisines. Over the years, I have see so many great restaurants come and go and when I found out there was open government data available, I thought I'd do some investigation. The main dataset I will use is the business licences dataset which consists of historical data on various businesses in Vancouver. I will also be using datasets that consist of bikeways, parking meters, schools, and libraries. All the data was gathered from [opendata.vancouver.ca](https://opendata.vancouver.ca/pages/home/). 

There is a lot of data to handle so I've decided to take this opportunity to learn Spark which is a distributed computing framework designed for big data. I will be using PySpark, the python API in order to run my analysis. The core of Spark relies on the idea of a cluster of nodes. A cluster of nodes allows us to partition our computation simultaneously amongst multiple nodes (which can be physical or virtual servers). This idea can also be extended to how Spark handles data, specifically called resilient distributed datasets (RDDs), in which the data is distributed.

I don't have the resource to run PySpark on multiple clusters so I will be running it locally, but I will nonetheless demonstrate a coherent data science workflow via PySpark. 

**Some questions I will attempt to answer:**
- What areas have particularly bad turnover?
- What type of restaurants/stores have a good chance of survival in a given area.
- What features of a restaurant/store helps its business? (how important social media is)
