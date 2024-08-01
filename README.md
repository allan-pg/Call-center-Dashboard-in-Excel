# Excel Call Center Data Analysis Dashboard
![Capture](https://github.com/user-attachments/assets/1672a2f7-f9b0-4e00-a56e-e662aa3ec491)

 

# Introduction  
This is a call center dashboard created with data from October 2020.  
It has over 30, 000 rows of data  

Tools used
- Pivot Tables
- Pivot Charts
- Slicer 
 
## pivot tables
A PivotTable is an interactive way to quickly summarize large amounts of data. You can use a PivotTable to analyze numerical data in detail, and answer unanticipated questions about your data.  

## pivot Charts  
PivotCharts complement PivotTables by adding visualizations to the summary data in a PivotTable, and allow you to easily see comparisons, patterns, and trends.

## Slicers  
Slicers provide buttons that you can click to filter tables, or PivotTables. Slicers are used to make your Dashboard an interactive Dashboard.

# Data Source
- What data is needed to achieve our objective?
We need Call Center data in excel/csv form that includes:
- calls by call center
- State calling from
- Reason for Calling
- Channel for calling
 
# Stages
- Design
- Developement
- Analysis

## Design
### Dashboard components required
- What should the dashboard contain based on the requirements provided?
To understand what it should contain, we need to figure out what questions we need the dashboard to answer:
  1. How many calls have been received in our call center?
  2. What is the reason for calling?
  3. What state are the customers calling from?
  4. How did the customers answer?
  5. What channels was the feedback received from?
  6. What was our response time to the calls?

For now, these are some of the questions we need to answer, this may change as we progress down our analysis.
## Development

What's the general approach in creating this solution from start to finish?
  1. Get the data
  2. Explore the data in Excel
  3. Clean the data with SQL
  4. Load the data into Power BI
  5. Generate the findings based on the insights
  6. Write the documentation + commentary
  7. Publish the data to GitHub Pages

## Data exploration notes
This is the stage where you have a scan of what's in the data, errors, inconcsistencies, bugs, weird and corrupted characters etc

- What are your initial observations with this dataset? What's caught your attention so far?
1. There are at least 6 columns that contain the data we need for this analysis, which signals we have everything we need from the file without needing to contact the client 
   for any more data.
2. The call_timestamp column contains incosistent dates i had to change the column to date type.
3. Call center column has both city and state in one column i split it into two columns City and State.
 
We have more data than we need, so some of these columns would need to be removed

## Data cleaning
- What do we expect the clean data to look like? (What should it contain? What contraints should we apply to it?)  
  The aim is to refine our dataset to ensure it is structured and ready for analysis.  
**The cleaned data should meet the following criteria and constraints:**  

- Only relevant columns should be retained.
- All data types should be appropriate for the contents of each column.  
- No column should contain null values, indicating complete data for all records.
 
## Findings
We discovered that
- Most of the sentiments are negative from our analysis
- Most of the callers called to inquire about billing
- Response time of the company is within the SLA
- Call center had the highest number of calls and web having the least number of calls
 
## Recommendations
- Increase number of employees in our call center in Los Angeles since most calls were enquired from Los Angeles CA.
- Find out on why most sentiments from our call centers are negative.
- Improve Billing system since billing is the most reason why we received calls.

