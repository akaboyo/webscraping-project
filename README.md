[companies.csv](https://github.com/user-attachments/files/17269140/companies.csv)# [TOP 100 COMPANIES IN THE US](#top-100-companies-in-the-us)

## Table of Contents
- [Project Overview](#project-overview)
- [Data Preprocessing Tools](#data-preprocessing-tools)
- [Data Analysis](#data-analysis)
- [Further Analysis Process](#further-analysis-process)
    - [Connecting to the Dataset in Tableau](#connecting-to-the-dataset-in-tableau)
    - [Data Preparation in Tableau](#data-preparation-in-tableau)
    - [Visualizations and Dashboards Creation](#visualizations-and-dashboards-creation)
    - [Insights and Interactivity](#insights-and-interactivity)
    - [Final Output and Sharing](#final-output-and-sharing)

## Project Overview

This project involves building a Python-based web scraper to collect data on the top 100 companies in the United States. The aim is to gather key information such as company names, industry sectors, and financial performance metrics and employee size, uncover key insights into industry distribution, geographic concentration, and growth patterns. The scraped data was exported to a csv file for further analysis, reporting, and integrated into financial dashboards with the objective of providing stakeholders with a deeper understanding of:

- The distribution of revenue across industries and states.
- Which industries and companies contribute the most to overall revenue and employee counts.
- How revenue growth varies across companies and industries, particularly identifying which sectors are growing fastest and which companies dominate their respective sectors.
- Identifying geographic trends in the location of company headquarters and state-level revenue distributions.
- What are the relationships between company size (in terms of employees) and revenue in different industries?

By answering these questions, this project aims to provide actionable insights to help businesses and analysts understand the economic landscape of the largest U.S. companies and identify opportunities for growth and investment.

## Data Preprocessing Tools
1. Web Scraping Libraries: In this project, i utilized these Python libraries:
   - BeautifulSoup: For parsing HTML content and extracting data from the webpage.
   - requests: For making HTTP requests to fetch the HTML content.
   - pandas: For cleaning and organizing the data in a structured format (dataframe) and exporting it to CSV.
  
3. Data Collection: The scraper fetches data on:
   - Rank 
   - Company Name
   - Industry Sector
   - Revenue (USD millions)
   - Revenue Growth
   - No. of Employees
   
4. Data Storage: The scraped data is cleaned and stored in a CSV structured format, for further analysis in Tableau.

## Data Analysis

Once collected, i analysed the data to find trends in industries, company performance, and created visual reports using Tableau.

This project showcases my practical web scraping, data handling, and analysis skills that can be applied to financial market research or business intelligence applications.
 
See below a snippet of the scraped data which was exported to a csv file for further analysis.
![Top 100 snippet](https://github.com/user-attachments/assets/165b6ed7-e540-4e8b-9641-7b7e08fc9e0c)

### View the Web-Scraping Process [here](https://www.kaggle.com/code/adebayoadebanjo/my-webscraping-project)


## Further Analysis Process

After completing the initial data preparation and exporting the cleaned dataset from Python, the next phase involved utilizing Tableau for in-depth analysis and visualization. 

### Connecting to the Dataset in Tableau
After exporting the cleaned CSV from Python, I connected Tableau to the dataset for further visualization. The data contains important columns like:
   - Rank
   - Company Name
   - Industry Sector
   - Revenue (USD millions)
   - Revenue Growth
   - No. of Employees

### Data Preparation in Tableau
Upon importing the dataset, I performed a few data preparation steps in Tableau:

- Created calculated fields for Positive Revenue growth and Negative Revenue growth with dynamic up and down arrows for distinguishing companies with positive and negative revenue growth rates and analyze operational efficiency across companies.
- Created parameters for Top 10 and Bottom 10 companies by Revenue(USD millions).
- Created sets for Top 10 and Bottom 10 companies by Revenue(USD millions).
- Geographic Data Preparation: Since the dataset didn’t include a "Country" column for generating maps, I created a calculated field for Country and set United States as the default country for all rows which was used to create a hierarchy for geographical locations.
- I splitted the Headquarters field into Area and State fields and changed the data type from strings to geographic roles for map visualization.
  
### Visualizations and Dashboards Creation
I focused on creating interactive dashboards that would allow stakeholders to explore different dimensions of the dataset. Here are some key visualizations featured:

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


## Insights and Interactivity
The dashboard allows users to:
- Use Action filters by industry, state, and company to explore granular detailed information.
- Hover over points on scatter plots, Map, and bar charts to view specific values for revenue, growth, and employee count.


## Final Output and Sharing
The interactive dashboards were published to Tableau Public for easy access and sharing with stakeholders. The insights from these visualizations provide a comprehensive understanding of the economic landscape of the top 100 U.S. companies by revenue, highlighting key sectors, geographic trends, and operational efficiencies.

[Click here to view dashboards](https://public.tableau.com/views/Top100USCompanies/Story1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)





