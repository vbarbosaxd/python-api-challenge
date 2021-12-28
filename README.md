# Python API Challenge
## Notes about files uploaded:
1. The **WeatherPy** folder only contains the image files of the plots created on Jupyter Lab and Matplotlib
2. The **output_data** folder only contains the cities.csv file used to generate the cities in WeatherPy
3. The **starter_code** folder contains both the WeatherPy and VacationPy jupyter notebooks, an empty API keys folder, and the csv file created in WeatherPy that was then used in VacationPy
4. The API keys were removed as a recommendation from the TA upon submission, so the grader will have to use their own API keys
## Project Overview
The goal of the project was to use my recent knowledge about Python requests, APIs, and JSON traversals to answer the question: *"What's the weather like as we approach the equator?"*

This project was split up into two parts: WeatherPy and VacationPy.
![equatorsign](https://user-images.githubusercontent.com/92385042/147614192-3806d52e-5fe2-41ef-8ffd-d6fe207f1f7d.png)

### WeatherPy
- I created a Python script that analyzed a file of more than 500 cities around the world and generated a separate file that used the OpenWeatherMap API to generate weather information for those cities.
- I then created a series of scatter plots to showcase the following relationships:
  1. Temperature (F) vs. Latitude
  2. Humidity (%) vs. Latitude
  3. Cloudiness (%) vs. Latitude
  4. Wind Speed (mph) vs. Latitude

- Then I ran a linear regression on each relationship, but separated the graphs into Northern and Southern Hemispheres:
  1. Northern Hemisphere - Temperature (F) vs. Latitude
  2. Southern Hemisphere - Temperature (F) vs. Latitude
  3. Northern Hemisphere - Humidity (%) vs. Latitude
  4. Southern Hemisphere - Humidity (%) vs. Latitude
  5. Northern Hemisphere - Cloudiness (%) vs. Latitude
  6. Southern Hemisphere - Cloudiness (%) vs. Latitude
  7. Northern Hemisphere - Wind Speed (mph) vs. Latitude
  8. Southern Hemisphere - Wind Speed (mph) vs. Latitude

### VacationPy
- Using jupyter-gmaps and the Google Places API, I tried to generate a heatmap of all the cities from the file I created in WeatherPy
- Then, I created a dataframe of all the cities that contain my ideal weather conditions and used Google Places API to find the nearest hotels to those locations
- Finally, I tried to generate a heatmap with the hotels pinned on top

![hotel_map](https://user-images.githubusercontent.com/92385042/147614157-96cc68c4-0bc7-4790-902b-73efe55f0aea.png)
