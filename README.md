
Weather App - Using Stack + API 
This project is a simple weather application using the OpenWeatherMap API to fetch and display current weather conditions and a short-term forecast based on user input. The function getWeather() is designed to retrieve real-time weather data for any city entered by the user and display the current temperature, description, and an hourly forecast.

Functionality Overview
getWeather()
The main function that handles:

Fetching current weather data and a 5-day hourly forecast for the given city.
Displaying the retrieved weather information on the web page.
Handling errors such as invalid city names.
Key Features:
Current Weather: Retrieves and displays temperature, weather description, and icon.
Hourly Forecast: Displays the temperature and weather icon for the next 8 hours.
User Input Validation: Ensures the user inputs a valid city before making the API request.
API URLs Used:
Current Weather API: Fetches the real-time weather data for the given city.
javascript
Copy code
const currentWeatherUrl = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}`;
Forecast API: Fetches the weather forecast data for the next 5 days (used to show the next 8 hours).
javascript
Copy code
const forecastUrl = `https://api.openweathermap.org/data/2.5/forecast?q=${city}&appid=${apiKey}`;


Weather App - getWeather Function
This project is a simple weather application using the OpenWeatherMap API to fetch and display current weather conditions and a short-term forecast based on user input. The function getWeather() is designed to retrieve real-time weather data for any city entered by the user and display the current temperature, description, and an hourly forecast.

Functionality Overview
getWeather()
The main function that handles:

Fetching current weather data and a 5-day hourly forecast for the given city.
Displaying the retrieved weather information on the web page.
Handling errors such as invalid city names.
Key Features:
Current Weather: Retrieves and displays temperature, weather description, and icon.
Hourly Forecast: Displays the temperature and weather icon for the next 8 hours.
User Input Validation: Ensures the user inputs a valid city before making the API request.
API URLs Used:
Current Weather API: Fetches the real-time weather data for the given city.
javascript
Copy code
const currentWeatherUrl = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}`;
Forecast API: Fetches the weather forecast data for the next 5 days (used to show the next 8 hours).
javascript
Copy code
const forecastUrl = `https://api.openweathermap.org/data/2.5/forecast?q=${city}&appid=${apiKey}`;
Display Functions
displayWeather(data)
This function handles displaying the current weather conditions:

City Name: Displays the name of the city.
Temperature: Displays the current temperature in Celsius.
Weather Description: A short description of the weather (e.g., cloudy, sunny).
Weather Icon: Displays an icon corresponding to the current weather condition.
displayHourlyForecast(hourlyData)
This function displays an 8-hour forecast:

Hour-by-Hour Weather: Shows the temperature for each hour.
Weather Icon: An icon representing the weather for each hour.
showImage()
This function ensures that the weather icon is displayed once data has been successfully fetched.
