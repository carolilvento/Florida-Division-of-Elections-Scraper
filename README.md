# Florida Division of Elections Scraper

This is a Python script that scrapes pages of election results from the Florida Division of Elections website. 

## Purpose & Context

The purpose of this scraper is to collect data on election results for various counties in Florida. It was made before the FL DOE officially released the elections results page, so this script is meant to find the pages to be scraped once results come out.

## How it works

The script uses the requests and BeautifulSoup libraries to download and parse the HTML content of the website. It then extracts the county name and precinct number from the URL, and prints the title of the HTML page. 

The scraper loops through a list of counties and ranges of election IDs, making requests to the Florida Division of Elections website for each combination of county and election ID. In order to find the pages urls of each county, it checks if the page exists through a return of a status code 200. The scraper then extracts the election results data from the HTML content of the response.

## Output

The script prints the county code, precinct number, and title of the HTML page for each valid URL it scrapes. 
