# World Oil Reserves Data Extraction, Validation, and Cleaning using Power BI

## Project Overview

This project demonstrates how to scrape, validate, and clean global oil reserve data from [Worldometers](https://www.worldometers.info/oil/) using Power BI. It covers extracting country-level oil reserves, their share of the world's total, and saving the processed data as a CSV file. A crucial aspect is data validation and cleaning steps to ensure the final dataset is accurate and ready for analysis.

---

## Problem Statement

Palm Spring Corp requires accurate and reliable global oil reserve data for strategic decision-making. They need to compare oil reserves across countries, assess each country's contribution to the global total, and identify trends. To fulfill this, the project extracts key data from [Worldometers](https://www.worldometers.info/oil/), validates its integrity, cleans any inconsistencies, and saves the refined data as a CSV for further analysis.

---

## Features

*   **Web Scraping**: Extracts country-wise oil reserve data from Worldometers.
*   **Data Transformation**:
    *   Cleans raw HTML content.
    *   Formats data into a structured table with columns for country name, oil reserves (in barrels), and world share (%).
*   **Data Validation**: Implements checks to ensure data accuracy and consistency.
*   **Data Cleaning**: Handles missing values, incorrect formats, and outliers.
*   **CSV Export**: Saves the validated and cleaned data as a CSV file.
*   **Dynamic Updates**: Allows easy refresh of data within Power BI.
*   **Visualization**: Creates interactive dashboards for comparative analysis.

---

## Tech Stack

*   **Power BI Desktop**:
    *   Web scraping via Power Query.
    *   Data Modeling and Visualization
    *   Data validation and cleaning
*   **Power Query (M Code)**:
    *   Used for HTML parsing, cleaning, validation, and transformation.
*   **CSV Export**:
    *   Saves transformed data.

---

## How It Works

1.  **Connect to Web Source**: Power BI connects to Worldometers using the "Get Data > Web" feature.
2.  **HTML Parsing**: Extracts the oil reserves table using Power Query's `Html.Table` function.
3.  **Data Validation**:
    *   **Type Validation**: Ensures correct data types for each column (e.g., numeric for oil reserves, text for country names).
    *   **Range Checks**: Verifies oil reserve values fall within reasonable limits.
    *   **Consistency Checks**: Checks for duplicate entries or inconsistencies between related fields.
4.  **Data Cleaning**:
    *   **Missing Values**: Handles missing values by imputation (filling with estimated values) or removal.
    *   **Format Standardization**: Standardizes formats for country names or date values.
    *   **Outlier Handling**: Identifies and addresses outliers, which could skew analysis.
5.  **CSV Export**: Saves the validated and cleaned data as a CSV file using Power BI’s capabilities or Python scripts.
6.  **Data Visualization**: (Optional) Creates visualizations in Power BI for data exploration.

---

## Input

![World Oil Statistic](https://github.com/user-attachments/assets/784ff42e-ca4c-4c4f-8520-a6b5dc3e965e)


---


## Output

![World Oil Preserved Data](https://github.com/user-attachments/assets/7794ec20-d3da-42c0-9db5-b2e7ef8b2b12)


---

## Setup Instructions

1.  Open Power BI Desktop.
2.  Use "Get Data > Web" and enter `https://www.worldometers.info/oil/`.
3.  In Power Query Editor:
    *   Extract the HTML table.
    *   Implement data validation steps (type checks, range checks, consistency checks).
    *   Implement data cleaning steps (handling missing values, standardizing formats, handling outliers).
4.  Load to Power BI's data model.
5.  To save as CSV: Open report view and put all column into values section. Then right-click 3 dot top right and saved as CSV file.

    

---

## Future Improvements

*   Automate updates via Power Automate or scheduled refreshes in Power BI Service.
*   Incorporate additional metrics.
*   Improve validation and cleaning processes.

---

## License

This project is licensed under the MIT License.
