The West Ham United vs. Chelsea match from the 2023/2024 Premier League season  was a highly anticipated fixture between two best English football clubs.

Date: August 20, 2023

Venue: London Stadium stadium, London city, England

Result: Chelsea 1-3 Liverpool 

The data has been scraped from https://www.sofascore.com/ 

Web Scraping with Beautiful Soup and Requests:
The code starts by importing the necessary libraries, requests for making HTTP requests and BeautifulSoup for web scraping.
It sends an HTTP GET request to the URL 'https://www.sofascore.com/chelsea-west-ham-united/MsN#11352418', pretending to be a web browser using the 'User-Agent' header.
It then parses the HTML content of the page using BeautifulSoup.

Selecting Elements with BeautifulSoup:
The code uses BeautifulSoup to select HTML elements with the attribute 'cursor' set to 'pointer' using the soup.select() method.

HTTP Headers:
It defines a dictionary of HTTP headers to be used in future requests, including 'accept', 'accept-language', 'user-agent', etc.

Making API Requests:
The code sends an HTTP GET request to 'https://api.sofascore.com/api/v1/event/11352418/shotmap' with the defined headers. This request is likely fetching data related to the shot map for the match.

Modifying Headers:
It updates the 'If-Modified-Since' header to a specific date.

Sending Another API Request:
Another HTTP GET request is sent to the same shot map API with the updated headers.

Processing and Visualizing Data:
The code imports additional libraries like pandas, matplotlib, mplsoccer, and openpyxl.
It reads data from an Excel file ('Book.xlsx') into a pandas DataFrame.
It creates a soccer pitch visualization using mplsoccer.
It plots goals, shots by West Ham United, and shots by Chelsea on the pitch.
The code also generates text annotations on the plot, including the total number of shots and the number of goals.
It reads data from another Excel file ('Book 1.xlsx') and calculates cumulative xG (expected goals) for both teams over time.
Finally, it plots the cumulative xG over the course of the match.
Overall, this code appears to scrape and visualize soccer match data, including shot maps and xG, using various Python libraries and data sources. The resulting output is visual representations of the match's key events and statistics.
