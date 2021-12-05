The repository contains the code analysing the weather of the randomly selected ~500 cities and script enabling to find the first hotel within 5000 meters from selected locations.

The WeatherPy file is utilising the OpenWeatherMap API to visualise the weather of 500+ cities and saves a CSV of all retrieved data. The plots included in the script showcase the following relationships:
- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude

The second part of the code devides the cities into Northern and Southern Hemisphere based on their latitudes as well as creates seperate plots and linear regressions on each relationship.


The VacationPy file uses the data retireved in the WeatherPy code and Google Places API to create a heat map that displays the humidity for every city. The script narrows the data based on the preferred weather conditions (temp. between 70 and 80 degrees, wind speed less than 10mph and 0% cloudiness). Then using Google Places API the code finds the first hotel within 5000 m from desired cities and plots hotels on top of the previous created heatmap.


The output_data folder contains the CSV file of raw cities data, PNG images of each scatter plot created in the WeatherPy and a screenshot of the heatmap and hotel markers created in the VacationPy.
