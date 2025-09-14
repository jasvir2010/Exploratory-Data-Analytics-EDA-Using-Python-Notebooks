# Exploratory Data Analytics (EDA) Using Python Notebooks

This repository contains a comprehensive exploratory data analysis (EDA) project for the hospitality domain using Python and Jupyter Notebooks. The analysis is performed on dummy hotel booking data, focusing on data cleaning, transformation, and insights generation.

## Datasets Used

All datasets are located in the `datasets/` folder:
- **dim_date.csv**: Date dimension table with day, month, year, week number, and day type.
- **dim_hotels.csv**: Hotel properties with IDs, names, categories, and cities.
- **dim_rooms.csv**: Room types and classes.
- **fact_aggregated_bookings.csv**: Aggregated bookings per property, date, and room category, including capacity.
- **fact_bookings.csv**: Individual booking records with guest count, booking status, revenue, ratings, and dates.
- **new_data_august.csv**: Additional booking data for August.

## Analysis Performed

- **Data Loading & Initial Exploration**: Previewed all datasets and noted key observations and data issues.
- **Data Cleaning**:
  - Fixed negative guest counts and outliers in revenue columns.
  - Handled missing values in capacity using median imputation.
  - Removed records where successful bookings exceeded capacity.
- **Data Transformation**:
  - Created `occupancy_percentage` to measure hotel utilization.
  - Merged datasets to enrich analysis with room class, hotel info, and date attributes.
  - Converted date columns to datetime, handling mixed formats.
- **Insights Generation**:
  - Average occupancy rate by room category and room class.
  - Average occupancy rate per city.
  - Occupancy comparison between weekdays and weekends.
  - City-wise occupancy for June and other months.
  - Revenue realized per city, hotel type, and booking platform.
  - Month-by-month revenue trends.
  - Average ratings per city.
  - Visualizations: Bar charts and pie charts for distributions and revenue shares.

## How to Run

1. Clone the repository.
2. Ensure all CSV files are present in the `datasets/` folder.
3. Open `hotel_analytics.ipynb` in Jupyter Notebook or VS Code.
4. Run the notebook cells sequentially to reproduce the analysis and visualizations.

## Requirements

- Python 3.x
- pandas
- matplotlib (for plots)
- Jupyter Notebook or VS Code

## Project Highlights

- Real-world EDA workflow: loading, cleaning, transforming, and analyzing data.
- Handling of mixed date formats and missing values.
- Insightful metrics for hotel performance and customer behavior.
- Ready-to-use code for similar hospitality analytics
