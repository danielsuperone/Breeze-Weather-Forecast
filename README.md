# 🌤️ Breeze Weather

A beautiful, minimal weather forecast application with interactive maps and comprehensive weather data.

![Weather App Preview](https://img.shields.io/badge/Status-Active-brightgreen) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)

## ✨ Features

### 🎯 Core Weather Data
- **Current Weather**: Real-time temperature, humidity, wind speed & direction
- **Feels Like Temperature**: Accurate perceived temperature
- **Atmospheric Data**: Pressure, visibility, and detailed conditions
- **Location-Based**: Automatic geolocation or manual city search

### 📊 Forecasts
- **Hourly Forecast**: Next 8 hours with detailed conditions
- **5-Day Daily Forecast**: Smart processing of daily highs/lows with expandable view
- **"Show More" Feature**: Toggle between compact and extended forecast view

### 🗺️ Interactive Weather Map
- **Real-time Weather Overlays**: 
  - 🌧️ Precipitation patterns
  - 💨 Wind speed and direction
  - ☁️ Cloud coverage
  - 📊 Atmospheric pressure
- **Dark Theme Integration**: Beautiful map styling that matches the app
- **Location Markers**: Visual indicators for current/selected locations
- **Smooth Layer Switching**: Seamless transitions between weather data

### 🌬️ Air Quality Monitor
- **AQI Index**: Real-time air quality measurements
- **Pollutant Breakdown**: PM2.5, PM10, and Ozone levels
- **Visual Indicators**: Color-coded air quality status
- **Health Recommendations**: Clear air quality descriptions

### 🎨 User Experience
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **Dark Theme**: Modern, eye-friendly interface
- **Unit Toggle**: Switch between Celsius/Fahrenheit
- **Location Modal**: User-friendly permission requests
- **Search Functionality**: Intelligent city/location search with autocomplete

## 🚀 Live Demo

[**View Live Demo**](https://danielsuperone.github.io/Breeze-Weather-Forecast)

## 📱 Screenshots

### Desktop View
![Desktop Screenshot](https://i.imgur.com/twDRYis.png)

### Mobile View
![Mobile Screenshot](https://i.imgur.com/U38SgKV.png)


### Interactive Map
![Map Screenshot](https://i.imgur.com/bklIOEl.png)
![Map Screenshot](https://i.imgur.com/buEZhQQ.png)

## 🛠️ Installation & Setup

### Prerequisites
- A modern web browser
- OpenWeatherMap API key (free tier works perfectly)

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/breeze-weather.git
   cd breeze-weather
   ```

2. **Get your API key**
   - Visit [OpenWeatherMap](https://openweathermap.org/api)
   - Sign up for a free account
   - Generate your API key

3. **Configure the API key**
   - Open `index.html`
   - Replace `YOUR_API_KEY_HERE` with your actual API key:
   ```javascript
   const API_KEY = 'your_actual_api_key_here';
   ```

4. **Launch the application**
   - Simply open `index.html` in your web browser
   - Or serve it using a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

### Deploy to GitHub Pages

1. **Enable GitHub Pages**
   - Go to your repository settings
   - Scroll to "Pages" section
   - Select "Deploy from a branch"
   - Choose `main` branch and `/root` folder

2. **Update API key for production**
   - Make sure your API key is properly configured
   - Commit and push your changes

## 🔧 Configuration

### API Endpoints Used
- **Current Weather**: `api.openweathermap.org/data/2.5/weather`
- **5-Day Forecast**: `api.openweathermap.org/data/2.5/forecast`
- **Air Pollution**: `api.openweathermap.org/data/2.5/air_pollution`
- **Geocoding**: `api.openweathermap.org/geo/1.0/direct`
- **Weather Maps**: `tile.openweathermap.org/map/{layer}/{z}/{x}/{y}.png`

### Customization Options

#### Weather Map Layers
```javascript
// Available weather layers
const weatherLayers = {
    precipitation: 'precipitation_new',
    wind: 'wind_new', 
    clouds: 'clouds_new',
    pressure: 'pressure_new'
};
```

#### Default Location
```javascript
// Change default fallback location (currently New York)
const DEFAULT_LAT = 40.7128;
const DEFAULT_LON = -74.0060;
```

#### Theme Colors
```javascript
// Customize colors in the Tailwind config
colors: {
    primary: '#0f172a',    // Dark blue background
    secondary: '#1e293b',  // Card backgrounds
    accent: '#38bdf8',     // Accent color (blue)
}
```

## 🏗️ Technical Stack

### Frontend Technologies
- **HTML5**: Semantic markup and structure
- **CSS3**: Custom styling and animations
- **JavaScript (ES6+)**: Modern vanilla JavaScript
- **Tailwind CSS**: Utility-first CSS framework

### APIs & Libraries
- **OpenWeatherMap API**: Weather data and forecasting
- **Leaflet.js**: Interactive maps and weather overlays
- **Geolocation API**: Automatic location detection
- **Font Awesome**: Beautiful weather icons

### Architecture
- **Single Page Application**: No build process required
- **Responsive Design**: Mobile-first approach
- **Progressive Enhancement**: Works without JavaScript for basic features
- **API-First**: Real-time data from OpenWeatherMap

## 📊 API Usage & Rate Limits

### Free Tier Limitations
- **1,000 calls/day**: Perfect for personal use
- **60 calls/minute**: Smooth user experience
- **5-day forecast**: Processed into smart daily summaries
- **Weather maps**: Unlimited tile requests

### Paid Tier Benefits
- **16-day daily forecast**: Direct daily API access
- **Historical data**: Weather history and statistics
- **Higher rate limits**: Enterprise-level usage
- **Priority support**: Faster API responses

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Ways to Contribute
- 🐛 **Bug Reports**: Found an issue? Let us know!
- 💡 **Feature Requests**: Have ideas for improvements?
- 🔧 **Code Contributions**: Submit pull requests
- 📖 **Documentation**: Help improve our docs
- 🎨 **Design**: UI/UX improvements and suggestions

### Development Setup
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Make your changes and test thoroughly
4. Commit your changes: `git commit -m 'Add amazing feature'`
5. Push to your branch: `git push origin feature/amazing-feature`
6. Open a Pull Request

### Code Guidelines
- Use consistent indentation (2 spaces)
- Add comments for complex logic
- Test on multiple browsers and devices
- Follow existing code style and conventions

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### MIT License Summary
- ✅ **Commercial use**: Use in commercial projects
- ✅ **Modification**: Modify and adapt the code
- ✅ **Distribution**: Share and distribute freely
- ✅ **Private use**: Use in private projects
- ⚠️ **Liability**: No warranty provided
- 📝 **License notice**: Include license in distributions

## 🙏 Acknowledgments

### APIs & Services
- **[OpenWeatherMap](https://openweathermap.org/)**: Comprehensive weather data
- **[Leaflet](https://leafletjs.com/)**: Open-source mapping library
- **[CartoDB](https://carto.com/)**: Beautiful map tiles

### Design & Assets
- **[Tailwind CSS](https://tailwindcss.com/)**: Utility-first CSS framework
- **[Font Awesome](https://fontawesome.com/)**: Icon library
- **[Google Fonts](https://fonts.google.com/)**: Inter font family

### Inspiration
- Modern weather applications and minimal design principles
- Progressive web app best practices
- Accessibility-first development approach

## 📞 Support & Contact

### Get Help
- 📋 **Issues**: [GitHub Issues](https://github.com/your-username/breeze-weather/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/your-username/breeze-weather/discussions)
- 📧 **Email**: your.email@example.com

### Community
- ⭐ **Star this repo** if you find it helpful!
- 🐦 **Follow me** on [Twitter](https://twitter.com/yourusername)
- 💼 **Connect** on [LinkedIn](https://linkedin.com/in/yourprofile)

---

<div align="center">

**Made with ❤️ by [Your Name](https://github.com/your-username)**

*If you found this project helpful, please consider giving it a ⭐!*

[![GitHub stars](https://img.shields.io/github/stars/your-username/breeze-weather?style=social)](https://github.com/your-username/breeze-weather/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/your-username/breeze-weather?style=social)](https://github.com/your-username/breeze-weather/network/members)

</div>
