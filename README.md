# Number of cities per country - SQL & Python Data Analysis

## Created by Patrycja Decowska
## Data source 
Sample database from SQL course

## Files in this project
- `cities_per_country` - dataset exported from SQL
- `SQL_script` - SQL quer
- `Visualization_Python` - upyter Notebook for final analysis and Python visualization
- `README.md` - describes this project
- `Licence` - MIT License for this project

## Main Goal 
To analyze and present the number of cities for each country in a given database.

## Description
I have combined SQL and Python to perform a simple data analysis. This project analyzes how many cities exist in each country using data
from a fictional SQL database.

### SQL Analysis
The country table is insufficient to store all of the information I need.
My query required data from two tables - country table and city table.

I have used aggregate function `COUNT` to count the numberof cities. 
`INNER JOIN` allows me to select data from two tables and `country_id` is the common field in both of them. 
Then I used `GROUP BY` in my code to take duplicate values and collect them together. 
`HAVING` clause allows me to filter the results. Thanks to this, I am able to see total number of cities for each country.

At the end of my code I used `ORDER BY` to sort in descending order by
number of cities and in ascending alphabetical order for countries.

**SQL clauses used in the code:** 
- `SELECT`
- `COUNT`
- `INNER JOIN`
- `GROUP BY`
- `HAVING`
- `ORDER BY`

**SQL Skills:**
- Joining multiple tables
- Aggregating data
- Filtering aggregated results
- Preparing data for further analysis and visualization

### Python Analysis & Visualization
I used Python for further analysis and visualization.
I have imported `pandas` and `matplotlib` libraries and uploaded the dataset
using `pd.read_csv`. I explored basic information, checked structure and
statistics. Afterwards, I created a bar chart to visualize the number of
cities per country.

## Results

The chart shows that India has the most cities in this database.
Moreover, Netherlands, Pakistan, Saudi Arabia, South Korea and Spain
have the lowest number of cities. - All of them have the same number of
cities.
