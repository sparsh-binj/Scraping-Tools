# Scraping-Tools

Python notebooks for scraping data from FBRef and NBA.com/stats, converting the scraped data into useful formats for further analysis. This project includes tools for scraping football (soccer) and basketball data using web scraping techniques and APIs, and saving the results in formats like CSV or Excel.

## Overview

This project provides two main scraping tools:
1. **FBRef Scraping Tool**: A Python script to scrape football statistics tables from the FBRef website, convert them into Pandas DataFrames, and save them as CSV or Excel files.
2. **NBA Stats Scraping Tool**: A script that uses the NBA API to gather shot chart data from NBA.com, processes the data, and combines it into a CSV or Excel file.

## FBRef Scraping Tool

The FBRef scraper pulls player stats from FBRef tables. It supports scraping multi-level column tables, such as defensive actions or player performance across various leagues. The scraper handles HTML comments, multi-level column headers, and other formatting challenges present on FBRef's pages.

### Features

- Scrapes tables from FBRef football statistics.
- Automatically cleans the data and removes unwanted columns.
- Can save data as CSV or Excel files.
- User-friendly: Simply modify the URL, table ID, and column drop list.

### How to Use

1. **Change URL and Table ID**: Modify Cell 7 in the notebook to include the URL of the FBRef page containing the table you want to scrape, and set the correct table ID.
2. **Run the Notebook**: Execute all cells to scrape the data, clean it, and save it as a CSV or Excel file.
3. **Preview**: After running the cells, you will see a preview of the scraped table in the notebook console.
4. **Save Data**: The table can be saved in either CSV or Excel format by modifying the file type in the save function.

### Requirements

- Python 3.7+
- Pandas
- Requests
- Selenium
- BeautifulSoup
- SeleniumBase
- ChromeDriverManager

## NBA Stats Scraping Tool

The NBA scraping tool uses the NBA API to pull detailed shot chart data from NBA seasons. It retrieves player and team statistics such as field goal attempts (FGA), makes, points scored, and more. This data is then processed into a Pandas DataFrame, cleaned, and exported as a CSV or Excel file for easy analysis.

### Features
- Gathers shot chart data for multiple NBA seasons.
- Combines data across multiple seasons into a single DataFrame.
- Cleans and formats columns for easy analysis, including mapping periods to quarters and converting dates.
- Saves data in CSV or Excel format.

### How to Use
1. **Modify Season**: Change the season values in the API requests to scrape data for different NBA seasons.
2. **Run the Script**: Run the script to fetch the shot chart data from NBA.com and process it into a Pandas DataFrame.
3. **Save Data**: After processing the data, save it as a CSV or Excel file for further analysis.

### Requirements
- Python 3.7+
- Pandas  
- NBA_API
- JSON
- Requests
- Datetime

## Future Enhancements
Expand the FBRef scraping tool to handle more complex table structures.
Add functionality to scrape data from additional basketball statistics endpoints.
Implement support for scraping multiple FBRef tables in a single run.
Optimize data handling for very large datasets in the NBA Stats scraper.

## Contributing
Feel free to open issues or submit pull requests if you'd like to contribute to this project. Feedback and improvements are always welcome!

## License
This project is licensed under the MIT License. See the LICENSE file for more details.


