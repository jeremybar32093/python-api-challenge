# python-api-challenge

This repository includes 2 parts: **WeatherPy** and **VacationPy**.

In **WeatherPy**, the [openweather api](https://openweathermap.org/api) in conjunction with the [citipy](https://pypi.org/project/citipy/) package to pull down weather information from a random sample of 500 cities (where available) as of a point in time. Data retrieved from the API calls are then pulled into a dataframe. Then, the following scatter plots are created listing relevant analysis:
* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Then, the dataframe is broken out further by northern hemisphere (>=0 degrees latitude) vs southern hemisphere (<0 degrees latitude). Using these breakouts, the following plots are created and also list relevant analysis. Additionally, a linear regression model was created for each plot:
* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

.PNG files of each plot along with corresponding analysis are saved in */output_data/plots/*.

**NOTE:** An API key is required to pull data from the [openweather api](https://openweathermap.org/api). While not pushed to the repo, this key is stored in a file called *api_keys.py* within the *WeatherPy* base directory. To run the code in the *WeatherPy.ipynb* file after pulling down, this file must be created and populated locally. 
