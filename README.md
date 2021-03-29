# Easyjet.com flights scraper
Python script scraping Easyjet flights for chosen airports

Script uses BS4 and parses JSON files from easyjet.com to get all future flights from specific origin to all listed destinations. Final script output is a CSV with name YYYYMMDD_n_months.csv based on script run date and number of selected months. 

Hard dependencies are `Selenium web driver`, `BeautifulSoup4` and `requests`.
Install required dependencies using `requirements.txt`

The script can be run two ways:
1. Within the command line
`python easyjet_scraper.py -d LJU LGW ABD -m 3` (-d: list of origin airports, -m: number of months for flights to be displayed)

2. Within Python IDE
Set variable `run_from_editor = True` and choose relevant airports and months in `"__name__" == __main__`


