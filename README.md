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

## Note

Please ensure you have the appropriate permissions and rights to scrape the website. Respect `robots.txt` and terms of service of the target website.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
