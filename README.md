# Weather App Pro 🌤️

A simple weather app that shows real-time weather for any city. Built with HTML, CSS, and JavaScript.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

## Features ✨

- Search weather for any city worldwide
- Shows temperature, humidity, and wind speed
- Beautiful animated weather icons
- Responsive design for mobile and desktop
- Error handling for invalid cities

## Quick Start 🚀

1. **Get an API key** from [OpenWeatherMap](https://openweathermap.org/api) (free)

2. **Clone this project**
   ```bash
   git clone https://github.com/yourusername/weather-app-pro.git
   ```

3. **Add your API key** - Open `index.html` and replace:
   ```javascript
   const apiKey = "YOUR_API_KEY_HERE";
   ```

4. **Add weather icons** - Put these GIF files in `images/` folder:
   - search.gif, clear.gif, clouds.gif, rain.gif
   - drizzle.gif, mist.gif, humidity.gif, wind.gif

5. **Open `index.html`** in your browser

## How to Use 📱

1. Type any city name (e.g., "London", "Tokyo", "Paris")
2. Click search or press Enter
3. See the weather with animated icons!

## File Structure 📁

```
weather-app-pro/
├── index.html     # Main file with HTML and JavaScript
├── style.css      # All the styling
├── README.md      # This file
└── images/        # Weather icons (GIF format)
```

## Technologies Used 💻

- **HTML5** - Structure
- **CSS3** - Styling and animations
- **JavaScript** - Fetching data and user interactions
- **OpenWeatherMap API** - Weather data

## Customization 🎨

**Change default city:**
```javascript
checkWeather("Berlin"); // Replace with your city
```

**Change colors:**
Edit the gradient in `style.css`:
```css
background: linear-gradient(135deg, #467446, #e04fa8);
```

## Support 📞

Having issues? 
- Check that your API key is correct
- Make sure all icon files are in the `images/` folder
- Open browser console (F12) to see error messages

## License 📝

MIT License - feel free to use this project!

---

⭐ **Star this repo if it helped you!** ⭐