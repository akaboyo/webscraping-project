# [TOP 100 COMPANIES IN THE US](#top-100-companies-in-the-us)

## Table of Contents
- [Project Overview](#project-overview)
- [Data Pre-processing Tools](#data-pre-processing-tools)
- [Data Analysis](#data-analysis)
- [Visual Insights](#visual-insights)
    - [Final Output and Sharing](#final-output-and-sharing)
    - [Technologies Used](#technologies-used)

## Project Overview

This project builds a **Python web scraper** to collect and analyze data on the top 100 companies in the United States. The main goal is to extract structured business data from a public source, clean it, and then visualize it using **Tableau** to uncover industry and geographic patterns.

### What’s Included

- Python scraper that extracts:
  - Rank
  - Company name
  - Industry sector
  - Revenue (USD millions)
  - Revenue growth (%)
  - Number of employees
  - Headquarters location

- Visuals created in Tableau:
  - Top 10 companies by revenue
  - Industry revenue share (Treemap)
  - Revenue vs Employee count (Scatterplot)
  - Revenue growth distribution (Box plot)
  - Geographic distribution of revenue (Map) 

## Data Pre-processing Tools
The scraper uses:

- **requests** — to fetch HTML pages
- **BeautifulSoup** — to parse and extract table data
- **pandas** — to clean and transform the data into a structured format (CSV/XLSX)

## Data Storage: 
The cleaned output is stored in `companies.xlsx` for analysis and visualization.
  
 ## Data Analysis

Once data is scraped and cleaned, it was imported into **Tableau**. Key steps included:

1. Creating calculated fields for metrics like positive/negative revenue growth.
2. Splitting geographic fields for map visualizations.
3. Building interactive dashboards to explore:
   - Sector contribution to total revenue
   - Company performance by revenue and workforce size
   - Growth trends and outliers
   - State business concentration patterns
     
See below a snippet of the scraped data which was exported to a csv file for further analysis.
![Top 100 snippet](https://github.com/user-attachments/assets/165b6ed7-e540-4e8b-9641-7b7e08fc9e0c)

#### View the Web-Scraping Process [on kaggle](https://www.kaggle.com/code/adebayoadebanjo/my-webscraping-project)


#### Download scraped dataset here [companies.xlsx](https://github.com/user-attachments/files/17280201/companies.xlsx)

### Visual Insights
Below are some of the visuals that communicate the project findings:

#### Industry and Company Performance Overview Dashboard
   - Bar Chart: Displaying total revenue of top 10 companies, highlighting the dominant sectors such as Retail, Petroleum, Financials and Healthcare.
   - Treemap: Showing revenue share by industry, allowing users to drill down into specific companies.   
![Top 10 companies](https://github.com/user-attachments/assets/ed5e9a50-5015-4071-91a3-eba2674a2f1a)
![Treemap](https://github.com/user-attachments/assets/918fa64b-2d37-449e-8d93-aef71d96bdd9)

#### Geographic Analysis Dashboard
   - Choropleth Map: Visualizing the distribution of top companies' headquarters across U.S. states and total revenue per state. States like California, Texas, and New York were identified as key business hubs.
![Map](https://github.com/user-attachments/assets/e8d3760c-6470-4e3b-9b19-3ffd9dd7a0c5)
   
#### Company Performance Dashboard
   - Scatter Plot: Plotting revenue vs. employee size by industry, highlighting outliers such as Amazon**, Walmart, and ExxonMobil, which have massive revenues and workforce.
   - Top N/Bottom N Companies: Featured a bar chart of the top 5 and bottom 5 companies by revenue growth(%).
   - Revenue Growth Distribution: A table visualizing the revenue growth distribution by state, industry, and company revealing that while some industries like Technology and 
     Healthcare have outliers with high growth, others are more stable.
![Scatterplot](https://github.com/user-attachments/assets/5a6a1492-9e7a-471d-a196-688bf5346f21)

![Box plot](https://github.com/user-attachments/assets/24345bd1-e16a-47eb-9a3c-982a42b6c5a6)

![Top and Bottom 5](https://github.com/user-attachments/assets/f1a9b02f-98ef-402c-b2bf-7e4a22ad8e89)

![Industry growth dist](https://github.com/user-attachments/assets/30693715-8cc5-406f-a95c-c26883d8e192)


These visuals help identify:
- High revenue companies dominating specific sectors
- Industry clusters with significant financial impact
- Correlation patterns between workforce size and revenue
- Geographic hubs of corporate activity

## Final Output and Sharing
The interactive dashboards were published to Tableau Public for easy access and sharing with stakeholders. The insights from these visualizations provide a comprehensive understanding of the economic landscape of the top 100 U.S. companies by revenue, highlighting key sectors, geographic trends, and operational efficiencies.

[Click here to view dashboards](https://public.tableau.com/views/Top100USCompanies/Story1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Technologies Used

- Python 3 (Requests, BeautifulSoup, pandas)
- Tableau Desktop
- CSV/XLSX for data exchange
- Git & GitHub for version control



