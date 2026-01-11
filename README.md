# New York City Airbnb Dashboard

## 📊 Project Overview
This interactive dashboard explores the Airbnb market in New York City. It combines geospatial analysis with comparative bar charts to help users understand pricing differences between boroughs (Manhattan, Brooklyn, Queens, etc.) and find listings within a specific budget.

## 🗂 Dataset
**Source:** New York City Airbnb Open Data
**Key Fields Used:**
- `Neighbourhood Group`: The 5 boroughs (Manhattan, Brooklyn, Queens, Bronx, Staten Island).
- `Price`: Nightly listing price.
- `Room Type`: Entire home vs. Private room.
- `Availability 365`: Number of days available per year.

## 🚀 Key Features
- **Budget Slider (Parameter Control):** A custom "Max Budget" slider allows users to filter out listings that are too expensive in real-time.
- **Dynamic Filtering:** A calculated field (`Price <= Max Budget`) links the slider to the map.
- **Cross-Filtering Dashboard:**
  - **Map:** Shows the density and location of listings.
  - **Bar Chart:** Compares average prices across boroughs.
  - *Action:* Clicking a borough on the map automatically filters the bar chart.

## 🛠 How It Was Built
1. **Parameter Creation:** Created an integer parameter for "Max Budget".
2. **Calculated Fields:** Built logic to link the parameter to the `Price` field.
3. **Dashboard Actions:** Configured the map to act as a filter for the rest of the dashboard.
4. **Visual Design:** Used a high-contrast color palette to distinguish price ranges (0–$500+).

## 💡 How to Use
1. **Set Your Budget:** Drag the "Max Budget" slider to see which listings remain available.
2. **Compare Boroughs:** Check the bar chart to see average price differences.
3. **Select a Region:** Click on area name on the map to isolate data for that area.
