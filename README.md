# HOTEL-DASBOARD
HOTEL DASBOARD
Project Overview
This project provides a comprehensive analysis of hotel booking data to uncover key performance indicators (KPIs) such as Total Revenue, Booking Trends, and Cancellation Rates. The goal is to help hotel management optimize their pricing strategy and improve operational efficiency through data-driven insights.
Key Features & Insights
Revenue Performance: Identified peak revenue months (Nov & Dec) and analyzed growth trends.
Cancellation Analysis: Tracked a 32.78% cancellation rate and correlated it with booking lead times.
Market Segmentation: Visualized revenue distribution across different channels like Online, Corporate, and Aviation.
Customer Preferences: Analyzed popular meal plans and room types to understand guest behavior.
Interactive Slicers: Dynamic filters for Date, Market Segment, and Room Types for real-time data exploration.
Tech Stack Used
Tool: Power BI Desktop
Data Cleaning: Power Query (ETL process)
Calculations: DAX (Data Analysis Expressions)
Data Source: Hotel Booking Dataset (CSV/Excel)
DAX Measures Used
Here are some of the key formulas created for this project:
TOTAL REVENUE
Total_Revenue = SUM('Hotel booking datasheet'[REVENUE])
CANCELLATION RATE 
Cancellation Rate = DIVIDE(COUNTROWS(FILTER('Hotel booking datasheet', 'Hotel booking datasheet'[booking_status] = "Canceled")), [Total Bookings], 0)
TOTAL GUESTS
Total Guests = SUM('Hotel booking datasheet'[no_of_adults]) + SUM('Hotel booking datasheet'[no_of_children])
