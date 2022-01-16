<h1 align="center">
  SPACBot
</h1>

A bot that scrapes the web and collects data from Reddit, Yahoo Finance, Google News, and SEC.gov on SPAC tickers and other SPAC-related news and information. Useful information is relayed to Discord to provide knowledge and alerts that can assist in SPAC investment.

**Warning:** The site used to create the list of SPACs has changed significantly and the bot most likely no longer functions correctly.

## Explanation

tableMaker.py compiles a list from spactrack.com (now spactrack.io) of notable SPACs based on certain criteria. This table is used by the other Python files that scrape different sites for information regarding these SPACs.

main.py contains the Discord bot notification sequence.

Note: All API tokens have been automatically reset and those contained in the code are simply for example.

## Features

proxy.py contains a list of proxies used by googlescrape.py to circumvent IP bans resulting from too many requests to Google.

## Dependencies

requests
BeautifulSoup4
shelve
urllib.request
lxml
