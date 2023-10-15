# Temperature Scraper and Visualizer

This project is aimed at scraping temperature data from a website and visualizing it using Streamlit.

## Files in the Project

1. `main.py` - This file contains the logic to scrape the temperature data from a specified URL and store it in an SQLite database.
2. `webapp.py` - This file is a Streamlit application to visualize the temperature data from the SQLite database.
3. `extract.yaml` - This file contains the SelectorLib configurations to extract data from the scraped webpage.

## Dependencies

- `requests`
- `selectorlib`
- `sqlite3`
- `streamlit`
- `plotly.express`

## How to Run

1. **Scraping and Storing Temperature Data**
    - Run `main.py`.
    - This will scrape the temperature data from the specified URL and store it in the SQLite database `data.db`.

\```bash
python main.py
\```

2. **Visualizing the Data**
    - Run `webapp.py` to start the Streamlit application.
    - This will display a line chart with date on the x-axis and temperature on the y-axis.

\```bash
streamlit run webapp.py
\```

## Configuration

- The target URL for scraping is set to `http://programmer100.pythonanywhere.com/`. You can change this in `main.py` if required.
- The `extract.yaml` file is configured to extract temperature using the CSS selector `#temperatureId > b`. Ensure this selector is valid for your target page or update it as needed.
