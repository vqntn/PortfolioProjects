# Urban Mobility Analysis using Google Places API

This project explores how mobility patterns in urban environments can be analyzed through location data using the Google Places API.  
The case study focuses on Concepción, Chile, combining point-based and territory-wide extraction methods to identify human activity trends at different times of the week.

---

## Goal

To develop a method to collect, filter, and visualize urban mobility data using the Google Places API.  
The project seeks to identify hourly popularity trends of places, aiming to provide useful insights for urban planning, transport optimization, and public infrastructure.

---

## Methodology

The project was conducted in two stages:

1. **Point-Based Search**  
   Specific known locations (e.g., shopping malls, parks, universities) were queried to retrieve `place_id` and obtain detailed metadata, including `populartimes`.

2. **Territorial Search Using a Polygon Grid**  
   A coordinate grid was created to cover an entire urban zone. Using radius-based searches around each point, hundreds of places were collected.  
   Not all returned data included `populartimes`, so a **data cleaning step** was introduced to retain only useful entries for temporal mobility analysis.

All collected data was processed using Python and exported for visualization in tools like Tableau and Kepler.gl.

---

## Key Features

- Place search via Google Maps API (place_id retrieval)
- Popular times extraction via `populartimes` library
- Geospatial grid querying for territory coverage
- Data cleaning and filtering
- Export to CSV/JSON for external visualization
- Analysis of urban mobility at hourly granularity

---

## Technologies Used

- **Python**
  - `pandas`, `requests`, `googlemaps`, `populartimes`, `matplotlib`, `seaborn`
- **Data Visualization**
  - Tableau, Kepler.gl
- **Jupyter Notebook** for documentation and analysis

---

## Results

- 100+ locations analyzed
- Peak activity patterns clearly identified for weekdays and weekends
- Generated dynamic dashboards and spatial maps showing urban activity cycles
- Demonstrated the value of using real-time and crowdsourced data for urban insights

---

## Files

- `Urban_Mobility_Analysis.ipynb`: full notebook with code, visuals, and explanations
- `data_input/`: raw place details from API
- `data_output/`: filtered places with populartimes
- `map_ready.csv`: file for direct upload into Kepler.gl

---

## 🔍 Next Steps

- Expand to multiple cities for comparative analysis
- Integrate mobility data with socioeconomic indicators
- Automate data extraction across time for longitudinal studies

---

## 🧑‍💻 Author

Valentina Quintana  
Data Analyst & Urban Data Enthusiast  
[LinkedIn](https://www.linkedin.com/in/vquintanao) • [GitHub](https://github.com/vqntn)

