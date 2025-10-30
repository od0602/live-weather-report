🌦️Weather & Air Quality Dashboard - Power BI





live-weather-report
------------------------------------------------------------------------------------------------------------------------------------------------------
This project showcases an interactive and visually appealing Weather & Air Quality Dashboard built with Power BI. It provides:

Real-time weather updates

7-day forecast visualization

Air Quality Index (AQI) insights with pollutant breakdowns

Dynamic DAX measures for category detection, color formatting, and health advisories


📊 Features
------------------------------------------------------------------------------------------------------------------------------------------------------
🌡 Temperature Details: Current temperature, weather condition, and city comparison

📅 7-Day Forecast Chart: Visual line chart showing temperature trends

🌇 Sunrise & Sunset Times

☁ Atmospheric Details: Humidity, Wind Speed, Visibility, Pressure, UV Index, and Precipitation

🏭 Air Quality Index (AQI): PM10, PM2.5, NO2, SO2, CO, and O3 pollutant levels

💡 AQI Suggestions: Health and safety recommendations powered by DAX

⚙️ Tech Stack

Power BI → Data modeling, visuals, and dashboard

DAX → Dynamic AQI logic (categories, color formatting & suggestions)

Custom Visuals → KPI cards, line charts, gauges, bar charts

CSV/JSON/API Data → Weather & AQI inputs


📌 Purpose
------------------------------------------------------------------------------------------------------------------------------------------------------
To deliver a real-time, data-driven solution that:

Informs users about current and forecasted weather

Raises awareness about air quality & health advisories

Supports informed outdoor planning & lifestyle decisions

🧠 Sample DAX Measure (AQI Suggestion)
------------------------------------------------------------------------------------------------------------------------------------------------------
AQI Suggestion =
VAR AQI = SELECTEDVALUE('Current'[Current_AQI])
RETURN
SWITCH(
    TRUE(),
    AQI <= 50, "Air is clean and healthy",
    AQI <= 100, "Acceptable air quality",
    AQI <= 150, "Sensitive groups should limit outdoor activities",
    AQI <= 200, "Limit prolonged outdoor exertion",
    AQI <= 300, "Avoid outdoor activities",
    "Stay indoors, wear a mask if outside"
)



Screenshort/ Demo
------------------------------------------------------------------------------------------------------------------------------------------------------
show what the dashboad looks like
Exampl:https://github.com/od0602/live-weather-report/blob/main/wather%20update.png
To get the latest report, please refresh the dashboard.
Note: The dashboard currently displays a 3-day weather forecast (instead of 7-day) due to free API subscription limits.
0 commit commentsComments0 (0)Lock conversation

🏷 Tags
------------------------------------------------------------------------------------------------------------------------------------------------------
#PowerBI #DataVisualization #WeatherDashboard #AQI #DAX #PortfolioProject
