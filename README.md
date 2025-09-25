# Weather App Pro 🌤️

A beautiful, responsive weather application that provides real-time weather information for cities worldwide. Built with vanilla HTML, CSS, and JavaScript using the OpenWeatherMap API.

![Weather App Preview](https://img.shields.io/badge/Status-Complete-brightgreen) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

## ✨ Features

- 🌍 **Search any city worldwide** - Get weather data for any location
- 🎨 **Beautiful gradient design** - Modern UI with smooth animations
- 📱 **Fully responsive** - Works perfectly on desktop, tablet, and mobile
- 🌦️ **Dynamic weather icons** - Icons change based on weather conditions
- ⚡ **Real-time data** - Live weather information from OpenWeatherMap API
- ❌ **Error handling** - User-friendly error messages for invalid cities
- 🔍 **Smart search** - Search by typing and pressing Enter or clicking the search button

## 🌦️ Weather Conditions Supported

- ☀️ **Clear Sky** - Sunny weather
- ☁️ **Clouds** - Cloudy conditions  
- 🌧️ **Rain** - Rainy weather
- 🌦️ **Drizzle** - Light rain
- 🌫️ **Mist** - Foggy/misty conditions

## 🚀 Demo

### What you'll see:
- **Temperature** in Celsius
- **City name** 
- **Humidity percentage**
- **Wind speed** in km/h
- **Weather icon** representing current conditions

## 📋 Prerequisites

Before running this project, you need:

- A web browser (Chrome, Firefox, Safari, etc.)
- Internet connection (for API calls)
- OpenWeatherMap API key (free registration required)

## 🛠️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/weather-app-pro.git
cd weather-app-pro
```

### 2. Get your API Key
1. Visit [OpenWeatherMap](https://openweathermap.org/api)
2. Sign up for a free account
3. Generate your API key
4. Copy the API key

### 3. Configure the API Key
Open `index.html` and replace the API key on line 35:
```javascript
const apiKey = "YOUR_API_KEY_HERE";
```

### 4. Add Weather Icons
Create an `images` folder and add these icon files:
- `search.png` - Search button icon
- `clear.png` - Clear sky weather icon
- `clouds.png` - Cloudy weather icon
- `rain.png` - Rainy weather icon
- `drizzle.png` - Drizzle weather icon
- `mist.png` - Mist weather icon
- `humidity.png` - Humidity indicator icon
- `wind.png` - Wind speed indicator icon

### 5. Run the Application
Simply open `index.html` in your web browser, or use a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

## 📁 Project Structure

```
weather-app-pro/
│
├── index.html          # Main HTML file
├── style.css          # CSS styling
├── README.md          # This file
│
└── images/            # Weather and UI icons
    ├── search.png
    ├── clear.png
    ├── clouds.png
    ├── rain.png
    ├── drizzle.png
    ├── mist.png
    ├── humidity.png
    └── wind.png
```

## 💻 Usage

1. **Default Loading**: The app loads with no city selected initially
2. **Search for a city**: Type any city name in the search box
3. **Get weather**: Click the search button or press Enter
4. **View results**: See temperature, humidity, wind speed, and weather icon
5. **Error handling**: Invalid city names will show a friendly error message

### Example searches:
- London
- New York  
- Tokyo
- Paris
- Mumbai

## 🔧 Technical Details

### Technologies Used
- **HTML5** - Structure and layout
- **CSS3** - Styling, gradients, and responsive design
- **JavaScript (ES6+)** - API integration and interactivity
- **OpenWeatherMap API** - Weather data source

### Key Features Implementation
- **Async/Await** for API calls
- **Fetch API** for HTTP requests
- **DOM manipulation** for dynamic content updates
- **Event listeners** for user interactions
- **Error handling** with try-catch and status codes
- **Responsive design** with CSS Flexbox

### API Integration
```javascript
// Example API call
const apiUrl = "https://api.openweathermap.org/data/2.5/weather?units=metric&q=";
const response = await fetch(apiUrl + city + `&appid=${apiKey}`);
```

## 🎨 Customization

### Change Default City
Uncomment and modify line 85 in `index.html`:
```javascript
checkWeather("Berlin"); // Replace "Berlin" with your preferred city
```

### Modify Colors
Edit the gradient in `style.css` line 11:
```css
background: linear-gradient(135deg, #467446, #e04fa8);
```

### Add More Weather Conditions
Extend the weather icon logic in `index.html` around line 45:
```javascript
else if(data.weather[0].main == "Snow"){
    weatherIcon.src = "images/snow.png";
}
```

## 📱 Browser Support

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ Mobile browsers

---

⭐ **If you found this project helpful, please give it a star!** ⭐