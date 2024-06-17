# NBA Player Salaries and Performance Analysis (2019-2022)

## Introduction
This project aims to analyze the relationship between NBA player salaries and their performance efficiency ratings (PER) for the 2019-2020, 2020-2021, 2021-2022, and 2022-2023 seasons. By using web scraping techniques to collect the necessary data, the project aims to find correlations between salaries and PER. The data is saved in CSV files for easy manipulation and potential further analysis.

## Objectives
- To demonstrate web scraping skills by collecting NBA player salary and performance data from the web.
- To save the scraped data in CSV files for further analysis.
- To find and interpret the correlation between player salaries and their PER.
- To visualize the relationship between salaries and PER using scatter plots with regression lines.

## Tools and Technologies
- **Python**: Main programming language used for the project.
- **Pandas**: For data manipulation and analysis.
- **Selenium**: For web scraping dynamic web pages.
- **BeautifulSoup**: For parsing HTML content.
- **Scipy**: For statistical analysis.
- **Matplotlib** and **Seaborn**: For data visualization.

## Methodology

### Step 1: Web Scraping Player Salaries
- Utilized the `requests` library to send GET requests to the HoopsHype website for the salary data of the 2019-2020, 2020-2021, 2021-2022, and 2022-2023 NBA seasons.
- Parsed the HTML content of the pages using `BeautifulSoup` to locate the table containing the player salaries.
- Extracted player names and corresponding salaries from the table.
- Stored the extracted data in lists and converted them into Pandas DataFrames.
- Saved each DataFrame as a CSV file with appropriate filenames.

### Step 2: Web Scraping Player Statistics
- Used the `Selenium` library to handle dynamic web pages on the NBA website for player performance statistics (PER) for the same seasons.
- Configured `Selenium` to run in headless mode and avoid sandbox restrictions.
- Waited for the required table to load on the page using explicit waits.
- Parsed the HTML content using `BeautifulSoup` to locate and extract player performance statistics.
- Calculate the PER for each player using the extracted statistics.
- Stored the data in Pandas DataFrames and saved them as CSV files.

### Step 3: Data Merging and Manipulation
- Loaded the previously saved CSV files containing player salaries and performance statistics.
- Merged the salary data across multiple seasons into a single DataFrame.
- Similarly, merged the performance statistics data across the same seasons.
- Combined the salary and performance DataFrames based on player names to create a comprehensive dataset.
- Converted salary values to millions of dollars for better readability.
- Saved the merged and manipulated data into new CSV files.

### Step 4: Correlation Analysis and Visualization
- Generated descriptive statistics for the combined dataset to understand the distribution of salaries and PER.
- Calculated the Pearson correlation coefficient and corresponding p-values between salaries and PER for each season.
- Visualized the relationship between salaries and PER using scatter plots with regression lines for each season.
- Saved the visualizations as image files for documentation and further analysis.

This methodology outlines the complete process from data collection through web scraping, data manipulation and merging, to the final correlation analysis and visualization, demonstrating a thorough approach to analyzing NBA player salaries and performance.
