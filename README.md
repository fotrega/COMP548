# Analysis of Income Inequality, Education, and Employment Trends

## Project Overview
This project explores the relationship between income inequality (GINI Index), education enrollment rates, and employment rates across countries and regions over time. The goal is to understand how education and employment influence income inequality and identify socio-economic patterns through clustering techniques.

### Income Inequality and Its Causes
Income inequality is a significant global issue, and understanding its causes and potential solutions is a critical area of study. This project examines how various factors like education and employment contribute to income inequality in different countries. We analyze trends in income inequality (measured using the GINI Index) and explore whether increased access to education and improved employment opportunities can reduce inequality.

### Main Objectives:
1. **Analyzing Income Inequality Trends**: Explore how income inequality (GINI Index) varies across countries and regions over time.
2. **Education and Inequality**: Investigate the relationship between education enrollment rates and income inequality.
3. **Employment and Inequality**: Analyze how employment rates influence income inequality.
4. **Clustering Countries**: Use clustering techniques to identify countries with similar socio-economic patterns, based on income inequality, education, and employment data.

## Data Sources

The primary dataset used in this analysis is the **World Development Indicators (WDI)** dataset, provided by the World Bank. This dataset includes socio-economic data for over 200 countries and regions, spanning multiple decades. Key indicators used in this analysis include:

- **GINI Index**: A measure of income inequality within a country.
- **Education Enrollment Rates**: Enrollment rates at various education levels.
- **Employment Rates**: Employment statistics for the labor force across various countries.

The dataset is publicly available via the World Bank API or can be downloaded in CSV format.

## Dataset Details

The project uses the following datasets:

- **WDICountry.csv**: Contains information about countries (e.g., country code, region, and income group).
- **WDISeries.csv**: Contains information about indicators (e.g., GINI Index, education, and employment data).
- **WDICSV.csv**: Contains the raw socio-economic data for various countries across years.

## Big Data Dimensions

This project addresses several key dimensions of Big Data:

- **Volume**: The data spans over 50 years and includes more than 1,600 indicators for over 200 countries.
- **Variety**: The dataset includes diverse socio-economic factors such as education, employment, income inequality, and health.
- **Veracity**: Some data points may have inconsistencies due to varying reporting standards across countries.
- **Value**: The insights derived from this analysis can influence policies and research in addressing global socio-economic issues.
- code addresses the Volume of the data (large-scale datasets across multiple decades and countries), the Variety of indicators (a mix of socio-economic factors), the Veracity of the data (handling inconsistencies and missing values), and the Value (providing actionable insights for policymakers and economists).

## Solution Overview

### Data Acquisition and Ingestion
The data is accessed using the World Bank API or by downloading CSV files directly. The data is then ingested into a NoSQL database (MongoDB) for efficient querying and processing. The MongoDB collections store data on countries, indicators, and socio-economic metrics.

### Data Processing and Cleaning
Data is cleaned and transformed using Python libraries such as Pandas and NumPy. The main steps in the data processing include:

1. **Reshaping the data**: The data is reshaped to a long format for easy analysis.
2. **Handling missing values**: Missing values are handled either by imputation (filling with the mean) or removal.
3. **Data filtering**: Data is filtered based on relevant keywords such as "GINI," "education," and "employment" to focus on the analysis.

### MongoDB Setup
The data is stored in a MongoDB database to facilitate efficient querying and storage. If you are running the project locally, ensure MongoDB is set up and running, or you can use a cloud-based service like MongoDB Atlas.

### Clustering and Analysis
- **Clustering**: The data is clustered using KMeans clustering to identify countries with similar socio-economic characteristics.
- **Statistical Analysis**: The correlation between various socio-economic factors, such as education and employment, is analyzed to understand their impact on income inequality.

## Hypotheses Tested

1. **Income Inequality Over Time**  
   We analyze how income inequality (GINI index) has evolved across countries and regions.

2. **Education and Income Inequality**  
   We investigate the correlation between education enrollment rates and income inequality, exploring whether increased education enrollment can help reduce income inequality.

3. **Employment and Income Inequality**  
   We examine whether higher employment rates are associated with lower levels of income inequality.

## Tools and Libraries Used

- **Programming Language**: Python
- **Libraries**:
  - **Pandas**: For data manipulation and analysis.
  - **NumPy**: For numerical operations.
  - **Matplotlib & Seaborn**: For data visualization.
  - **Scikit-learn**: For machine learning and clustering techniques.
  - **PyMongo**: For interacting with MongoDB.
  - **Jupyter Notebook**: For running the code and displaying results interactively.



