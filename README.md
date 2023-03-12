# Web_scraping_project

## Introduction

Web srarping is a technique used to collect content and data from internet.This data is usually saved in a local file so that it can be manipulated and analyzed as needed.

Web scraping is done by Making an HTTP request to a server. Extracting and parsing the website’s code. Saving the relevant data locally

![web scrape](https://user-images.githubusercontent.com/122099372/224527455-2512e6a4-8bd3-4845-8a9b-9babdf2a485d.png)

## Web scraping 

In this project I have used Amazon website to scrape data and converted it into csv file.

Firstly, I have used following python libraries:

    1. BeautifulSoup
    2. requests
    3. Pandas
    4. Numpy
    
After importing these libraries I have sent a HTTP request from my local machine to amazon server using 'requests' package.

With the approval of request I have converted the websit content format from bytes to html format using 'BeautifulSoup'.

Then I have fetched all the links from html code using find_all function in BeautifulSoup. From these links getting href and making aproper link by adding 'https://www.amazon.com'.

In the same way I have fetched title of the product, Price, rating,review and availability of the product by using for loop from the html code. then stored into a dictionary.

NOw using pandas and numpy libraries  I cleaned the data and converted in into a csv file.
