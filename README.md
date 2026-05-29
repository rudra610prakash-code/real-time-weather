# 🌤️ Real-Time Weather App

A beautiful, real-time weather application built with vanilla **JavaScript**, **HTML5**, and **CSS3**. Get instant weather updates for any city in the world with an intuitive and modern user interface.

---

## ✨ Features

- 🔍 **Search Weather by City** - Type any city name and get instant weather information
- 🌡️ **Real-time Temperature** - Displays current temperature in Celsius
- 💧 **Humidity Tracking** - Shows current humidity percentage
- 🌪️ **Wind Speed** - Displays wind speed in km/h
- 🎨 **Dynamic Weather Icons** - Changes based on weather conditions (Clouds, Clear, Rain, Drizzle, Mist)
- ❌ **Error Handling** - Validates city names and shows error messages for invalid inputs
- 🎯 **Modern UI/UX** - Beautiful gradient design with smooth interactions

---

## 🎨 UI/UX Design Highlights

### **Design Philosophy**
The application follows modern design principles to provide an exceptional user experience:

### **Visual Elements**

- **Gradient Background**: Eye-catching gradient from turquoise (#00feba) to deep purple (#5b548a)
- **Card-Based Layout**: Clean, centered card design with maximum width for optimal readability
- **Color Scheme**: 
  - Primary: Vibrant gradient
  - Text: Clean white for contrast
  - Input Fields: Light background (#ebfffc) with dark text
  
- **Typography**: Uses 'Poppins' font family for modern, readable text at various weights

### **Interactive Elements**

- **Search Input**: 60px height with rounded corners for easy interaction
- **Search Button**: Circular design with hover cursor feedback
- **Weather Display**: Large, readable temperature display (80px font)
- **Info Sections**: Two-column layout for humidity and wind speed information

### **User Experience**

1. **Intuitive Search**: Users can simply type a city name and click search
2. **Instant Feedback**: Weather data loads immediately after search
3. **Error Messages**: Clear error handling for invalid city names
4. **Visual Hierarchy**: Important information (temperature) is prominently displayed
5. **Accessibility**: Good contrast ratios and readable font sizes

### **Responsive Design**

```
Desktop: 470px max-width card with full spacing
Tablet: Adjusts to screen size with 90% width
Mobile: Optimized layout maintaining usability
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| **HTML5** | Structure and semantic markup |
| **CSS3** | Styling, gradients, and responsive design |
| **JavaScript** | Dynamic functionality and API integration |
| **OpenWeatherMap API** | Real-time weather data |

---

## 🚀 How to Use

### **Installation**

1. Clone the repository:
```bash
git clone https://github.com/rudra610prakash-code/real-time-weather.git
cd real-time-weather
```

2. Open `index.html` in your web browser:
```bash
# On macOS
open index.html

# On Windows
start index.html

# On Linux
xdg-open index.html
```

### **Usage**

1. Enter a city name in the search box
2. Click the search button or press Enter
3. View the weather information instantly:
   - Current temperature
   - Humidity percentage
   - Wind speed
   - Weather condition icon

---

## 📁 File Structure

```
real-time-weather/
├── index.html          # Main HTML structure
├── style.css           # Styling and responsive design
├── script.js           # JavaScript functionality
├── Images/             # Weather icons and assets
│   ├── clouds.png
│   ├── clear.png
│   ├── rain.png
│   ├── drizzle.png
│   ├── mist.png
│   ├── humidity.png
│   ├── wind.png
│   ├── search.png
│   └── sigma.jpeg
└── README.md           # Documentation
```

---

## 💻 Code Overview

### **HTML Structure**

```html
<div class="card">
  <div class="search">
    <input type="text" placeholder="Enter city name">
    <button><img src="Images/search.png" alt="search"></button>
  </div>
  <div class="weather">
    <!-- Weather information displayed here -->
  </div>
</div>
```

### **JavaScript Logic**

The `script.js` file handles:

1. **API Integration**: Fetches weather data from OpenWeatherMap API
2. **City Search**: `checkWeather()` function processes user input
3. **Dynamic Icon Selection**: Changes weather icon based on conditions
4. **Error Handling**: Shows error message for invalid cities
5. **Data Display**: Updates DOM with real-time weather information

**Key Function:**
```javascript
async function checkWeather(city){
    const response = await fetch(apiUrl + city + `&appid=${apiKey}`);
    // Fetch and display weather data
}
```

### **CSS Styling**

- **Flexbox Layout**: Used for centering and component alignment
- **Border-radius**: Creates modern rounded corners
- **Box-shadow**: Adds depth with glowing effects
- **Gradients**: Linear gradient for background and card styling
- **Media Queries**: Ensures responsive design across devices

---

## 🌐 API Integration

This app uses the **OpenWeatherMap API** to fetch real-time weather data:

- **Endpoint**: `https://api.openweathermap.org/data/2.5/weather`
- **Units**: Metric (Celsius)
- **Data Returned**:
  - Temperature (main.temp)
  - Humidity (main.humidity)
  - Wind Speed (wind.speed)
  - Weather Condition (weather[0].main)

---

## ⚠️ Error Handling

The app gracefully handles errors:

- **Invalid City**: Shows "Invalid city name" error message
- **Network Issues**: Displays appropriate feedback
- **Hidden Elements**: Error message hides automatically when valid data is found

---

## 🎯 Key Features in Detail

### **Dynamic Weather Icons**
```javascript
if(data.weather[0].main == "Clouds"){
    weatherIcon.src = "images/clouds.png";
}
// ... more conditions for different weather types
```

---

## 🔐 Security Notes

- API key is stored in the client-side code for this demo
- For production, use environment variables and backend proxy
- Consider implementing rate limiting

---

## 🚧 Future Enhancements

- [ ] Add weather forecasts (5-day, weekly)
- [ ] Implement geolocation-based weather
- [ ] Add favorite cities feature with local storage
- [ ] Dark/Light theme toggle
- [ ] Weather alerts and notifications
- [ ] Historical weather data
- [ ] Air quality index display
- [ ] Multiple language support

---


## 🎨 Color Palette

| Color | Usage |
|-------|-------|
| #00feba | Gradient start |
| #5b548a | Gradient end |
| #222 | Background |
| #fff | Text |
| #ebfffc | Input background |
| #555 | Input text |

---

## 📝 Getting Started

1. **Prerequisites**: Modern web browser (Chrome, Firefox, Safari, Edge)
2. **No Installation Needed**: Just open `index.html`
3. **Internet Required**: For API calls to OpenWeatherMap

---

---

## 📸 Screenshot
<img width="1294" height="557" alt="image" src="https://github.com/user-attachments/assets/607996ec-ffdb-4f59-9b74-9df5fc22a53e" />



---

## 👨‍💻 Author

**Rudra Prakash**
- GitHub: [@rudra610prakash-code](https://github.com/rudra610prakash-code)


---
