# UBER Trip Analysis

This Power BI dashboard project is designed to help Uber stakeholders—such as operations managers, data analysts, and decision-makers—gain actionable insights from trip data. It provides a deep dive into booking trends, customer behavior, trip efficiency, and geographical demand distribution.

With multiple dashboards (Overview, Time Analysis, and Details Tab), the project enables real-time performance monitoring and data-driven strategic decisions. The insights include total and average bookings, revenue, trip distance and time, vehicle type preferences, and booking patterns across days and hours. Advanced interactive features like dynamic measure selectors, slicers, drill-throughs, tooltips, and bookmarks enhance usability and exploration.

# Uber Trip-Dashboard

### Dashboard Link :https://app.powerbi.com/view?r=eyJrIjoiZGUzZTczNjMtNTUyMy00NDI5LWFmYzMtYmJhZGFhZGM0MDdjIiwidCI6IjkxODMwYzY4LTkwMzgtNDM3Mi04N2U2LWNhMTk3N2VlNDNiOCJ9

## Problem Statement

This dashboard helps Uber better understand its riders’ booking behavior, trip patterns, and operational efficiency. It allows the company to identify areas of improvement by analyzing total trips, revenue, trip durations, vehicle preferences, and time-based demand patterns.


### Steps followed 

-Step 1: Load the Excel file containing Trip Details and Location Table into Power BI Desktop.

-Step 2: Open Power Query Editor to inspect and clean the data tables.

-Step 3: In the View tab, enable Column Quality, Column Profile, and Column Distribution.

-Step 4: Check for nulls or duplicates, especially in key columns like Trip ID and Fare Amount.

-Step 5: Apply necessary data transformations and close Power Query Editor to load data into the model.

-Step 6: In the Model View, create relationships between PULocationID and Location ID.

-Step 7: Create another relationship between DOLocationID and Location ID.

-Step 8: Add a new calculated column Pickup Date using the DAX formula to extract date from Pickup Time.

-Step 9: Create a new Calendar Table using the CALENDAR() function with the pickup date range.

-Step 10: Link the Calendar Table to the Pickup Date column in the Trip Details table.

-Step 11: Choose a clean and professional report theme from the View tab for dashboard styling.

-Step 12: Create DAX measures like Total Bookings, Total Booking Value, and Average Trip Distance.

-Step 13: Create a DAX measure for Average Trip Time using DATEDIFF() between pickup and drop-off.

-Step 14: Use DAX variables to format the total trip distance into "K Miles".

-Step 15: Design Dashboard 1: Overview with KPIs like bookings, revenue, and trip time.

-Step 16: Add Dashboard 2: Trip Distance Analysis using bar and line charts.

-Step 17: Add Dashboard 3: Location & Vehicle Insights with maps and visuals by city and vehicle.

-Step 18: Insert slicers for filtering data by city, vehicle type, payment method, etc.

-Step 19: Use card visuals for key metrics like average trip time and total revenue.

-Step 20: Finalize your dashboard with proper formatting, titles, and tooltips for better user experience.
   
# Insights
A three page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

- **Peak Hours**: 5 PM – 8 PM, especially on Fridays and weekends
- **Hot Zones**: Downtown and Midtown (pickups), airports/corporate hubs (drop-offs)
- **Revenue Drivers**:
  - High revenue from commercial zones
  - Best fare/time ratio from 3–8 km trips
- **Trip Characteristics**: Average duration ~15–20 mins
- **Low Activity**: 2 AM – 5 AM

---

##  Business Solutions

Based on the insights, the following recommendations were made:

- Optimize **driver allocation** using demand patterns
- Apply **dynamic pricing** during high-demand periods
- Launch **promotions** in low-demand areas
- Focus on **expanding operations** in top-performing zones
- Improve **route optimization** for long-duration trips
- Set up **weekly dashboards** for ongoing monitoring

---

## Tools Used

- **Power BI** – Data modeling, dashboarding, and insights
- **Excel** – Data cleaning and preparation
- **Power Query** – Data transformation
- **DAX** – Measures and calculated columns
- **Map Visuals** – Geolocation-based insights

---

##  Conclusion

The Uber Trip Analysis project demonstrates how businesses can convert raw data into valuable insights using tools like Power BI. From understanding rider patterns to optimizing driver allocation and maximizing revenue, this dashboard can guide data-driven decision-making for any ride-sharing platform.

---

##  Project Structure

```bash
Uber-Trip-Analysis/
│
├── 📁 Dataset/
│   ├── Uber_Trips.csv
│   └── Location_Data.csv
│
├── 📊 PowerBI_Dashboard.pbix
│
├── 📄 README.md
