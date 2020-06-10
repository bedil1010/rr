## Avocado Analysis 

### Files:

* `avocado.RData`: RData with preprocessed data
* `avocado.Rmd`: description of dataset as Rmd
* `avocado.Proj`: description of dataset as Proj
* `avocado.csv`: csv version of dataset 
* `README.md`: description of the project as github README
* `main_last.Rmd`: Description of project with with ui and server shiny application
* `src`: input images used in the app


### Packages:
`ggplot2`, `tidyr`, `dplyr`, `lubridate`, `tibbletime`, `shiny`, `tidyverse`, `rvest`, `magrittr`, `ggmap`, `stringr`, `usmap`, `gtrendsR`, `shinyWidgets`.


## Dataset

This data was downloaded from the Hass Avocado Board website in May of 2018 & compiled into a single CSV. Here's how the Hass Avocado Board describes the data on their website:

The table below represents weekly 2018 retail scan data for National retail volume (units) and price. Retail scan data comes directly from retailers’ cash registers based on actual retail sales of Hass avocados. Starting in 2013, the table below reflects an expanded, multi-outlet retail data set. Multi-outlet reporting includes an aggregation of the following channels: grocery, mass, club, drug, dollar and military. The Average Price (of avocados) in the table reflects a per unit (per avocado) cost, even when multiple units (avocados) are sold in bags. The Product Lookup codes (PLU’s) in the table are only for Hass avocados. Other varieties of avocados (e.g. greenskins) are not included in this table.

Avocados Are a Heart-Healthy, Nutrient-Dense Superfood   Nutrient-dense foods are those that provide substantial amounts of vitamins, minerals and other nutrients with relatively few calories. One-third of a medium avocado (50 g) has 80 calories and contributes nearly 20 vitamins and minerals, making it a great nutrient-dense food choice."


- The dataset can be found on: https://www.kaggle.com/neuromusic/avocado-prices
- Which was collected from: https://hassavocadoboard.com/

## Features
- `Date` - The date of the observation
- `AveragePrice` - the average price of a single avocado
- `type` - conventional or organic
- `year` - the year
- `Region` - the city or region of the observation
- `Total Volume` - Total number of avocados sold
- `4046` - Total number of avocados with PLU 4046 sold
- `4225` - Total number of avocados with PLU 4225 sold
- `4770` - Total number of avocados with PLU 4770 sold

## The App

In our app we are using avocado dataset from kaggle.com. We are doing an exploratory data analysis using Shiny package where firstly have a map where and two types of graph: scatter plot and bar plot where we observe the relationship between some of the feature of the dataset.

### Map

- Map of the avocado consumption in US in different states

### Scatter plot
- The relationship of the various features (numerical) of the dataset as:

    - Date vs Average price
    - Volume vs price + types
    - Simple linear regression for Price vs Volume
    
### Bar plot
- Checking the density of different features (numerical) 
    - with respect to factor features
