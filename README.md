# Weather App

## Description

This is a simple, responsive weather application built with HTML, CSS (using Tailwind CSS), and JavaScript. It fetches real-time weather data from the Open-Meteo API and displays current weather conditions, hourly forecasts, daily forecasts, and interactive charts. The app supports searching for cities, using the user's current location, and toggling between Celsius and Fahrenheit units.

## Features

- **Current Weather Display**: Shows the current temperature, condition, location, and time with a corresponding weather icon.
- **Forecast Tabs**: 
  - Today: Hourly forecast in a vertical list.
  - Tomorrow: Hourly forecast for the next day in a vertical list.
  - Next 7 Days: Daily forecast with high/low temperatures in a vertical list.
- **Unit Toggle**: Switch between °C and °F.
- **Search Functionality**: Search for weather by city or airport name.
- **Geolocation Support**: Automatically fetches weather for the user's current location (with fallback to San Francisco if denied).
- **Charts Screen**: 
  - Hourly temperature line chart.
  - Daily high/low bar chart.
  - Separate unit toggle for charts.
- **Responsive Design**: Optimized for mobile views with fixed navigation at the bottom.
- **Error Handling**: Displays errors for invalid searches or API failures.

## Technologies Used

- **HTML5**: Structure of the application.
- **Tailwind CSS**: Styling and responsive design.
- **JavaScript**: Logic for API calls, DOM manipulation, and event handling.
- **Chart.js**: For rendering interactive charts.
- **Open-Meteo API**: For weather data and geocoding.
- **Nominatim (OpenStreetMap)**: For reverse geocoding to get city names from coordinates.
- **SVG Icons**: Phosphor icons for weather representations.

## Setup and Installation

1. **Clone or Download**: Download the HTML file or clone the repository if hosted.
2. **Dependencies**: 
   - The app uses CDN links for Tailwind CSS and Chart.js, so no local installation is required.
   - Ensure you have a modern web browser (Chrome, Firefox, etc.).
3. **Run the App**: Open the `index.html` file in your browser.

No server is needed as it's a client-side application.

## Usage

1. **Home Screen**:
   - The app loads with the current location's weather (or San Francisco as default).
   - Search for a city in the input field and press Enter to update.
   - Toggle between forecast tabs (Today, Tomorrow, Next 7 Days).
   - Switch units with the °C/°F button.

2. **Charts Screen**:
   - Navigate via the bottom tab.
   - View hourly or daily charts.
   - Toggle chart units independently.

3. **Navigation**:
   - Fixed bottom tabs for Home (Weather) and Charts.

## Limitations

- Relies on free APIs; rate limits may apply.
- Geolocation requires user permission.
- Forecasts are limited to 24 hours for today/tomorrow and 7 days for weekly.
- No persistent storage; refreshes data on load/search.

## Credits

- **APIs**: Open-Meteo for weather and geocoding, Nominatim for location names.
- **Libraries**: Tailwind CSS, Chart.js.
- **Icons**: Based on Phosphor icons (SVG paths included in code).

## License

This project is open-source and available under the MIT License. Feel free to use, modify, and distribute.
