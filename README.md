# Air-Quality-Report-in-Power-BI

## Project Overview
This Power BI dashboard provides a comprehensive analysis of the air quality across multiple Indian cities using pollutant data collected over time. The aim of the project is to help users understand which environmental parameters most significantly impact the Air Quality Index (AQI), and visualize pollution trends across regions.

The project includes dynamic visualizations that allow users to explore pollution levels, compare cities, and monitor key pollutants such as PM2.5, PM10, NO₂, CO, NH₃, SO₂, and more.

## Features
AQI Trend Analysis over time using a line chart

City-wise Air Quality Ranking (Top 3 most polluted and least polluted cities)

Slicer for City Selection to dynamically filter and compare regions

Parameter Monitoring Cards for key pollutants:

Carbon Monoxide (CO)

Nitrogen Dioxide (NO₂)

Sulfur Dioxide (SO₂)

PM2.5 (Particulate Matter <2.5 μm)

Map View for geographical AQI distribution

Dynamic Filters & Slicers for interactive exploration

Auto-refresh Date Indicator showing last data update

Clean, Responsive Layout with title, formatting, and consistent visual alignment

## Dataset Information
Source: Publicly available Indian air quality dataset

Format: CSV (cityor_data.csv)

Fields Include:

Date, City, PM2.5, PM10, NO, NO₂, NOx, NH₃, CO, SO₂, O₃, Benzene, Toluene, AQI

Date Range: January 2015 – July 2020

## How to Use
Open Power BI Desktop

Connect to the dataset via Get Data > SharePoint Folder

Transform data:

Remove nulls and unnecessary columns

Use "First Row as Headers"

Replace Sum aggregations with Average

Load the cleaned data into Power BI

Create visualizations:

Line Chart: AQI over time

Bar Charts: Top 3 and Bottom 3 polluted cities

Slicers: City filters

Cards: Key pollutant averages

Map: AQI by city bubble chart

Format visuals and layout with:

Background shading

Borders and shadows

Title and labels

Add a Last Refresh Date using a custom DAX measure:

Last Refresh Date = "Last Refresh Date: " & MAX('Table'[Date])
