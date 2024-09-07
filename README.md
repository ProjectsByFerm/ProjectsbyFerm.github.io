Weather App - Using OpenWeatherMap API
This project is a simple weather application that utilizes the OpenWeatherMap API to retrieve and display real-time weather information and a short-term forecast based on user input.

Core Functionality:

getWeather() Function:
Fetches current weather data and a 5-day hourly forecast for a specified city.
Displays retrieved information on the web page.
Handles errors for invalid city names.
Key Features:
Current Weather: Displays temperature, weather description, and icon.
Hourly Forecast: Presents temperature and weather icon for the next 8 hours.
User Input Validation: Ensures valid city input before making API requests.
API Usage:
Current Weather API: Retrieves real-time data for the specified city (URL example included).
Forecast API: Retrieves weather forecast data for the next 5 days (used to display the next 8 hours) (URL example included).
Display Functions:

displayWeather(data): Handles displaying current weather conditions:
City Name
Current Temperature (Celsius)
Weather Description
Weather Icon
displayHourlyForecast(hourlyData): Displays an 8-hour forecast:
Hour-by-Hour Weather (Temperature)
Weather Icon for Each Hour
showImage(): Ensures successful data retrieval before displaying the weather icon.
Additional Notes:

Consider removing the repeated description and functionality overview for the project.
Replace javascript with the actual programming language used for clarity.
Omit the actual API URLs for security reasons. Mention they are constructed using the OpenWeatherMap API format with placeholders for city and apiKey.
You can add information about how to set up the API key or any dependencies required to run the project.
