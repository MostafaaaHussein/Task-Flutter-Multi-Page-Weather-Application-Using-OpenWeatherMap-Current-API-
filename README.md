
# 🌦️ Flutter Weather App

A multi-page Flutter mobile application that retrieves and displays real-time weather data using the OpenWeatherMap API.  
This project demonstrates **REST API integration**, **state management using Provider**, **local storage with SharedPreferences**, and **clean architecture principles**.

---

## 📱 App Description

The application allows users to search for current weather conditions in any city worldwide.  
It provides detailed weather metrics such as:

- Current Temperature & "Feels Like"
- Weather Description & Icon
- Humidity & Pressure
- Wind Speed
- Sunrise & Sunset times (formatted to local time)
- Local time calculation based on timezone offset

Users can also save favorite cities for quick access and switch between **Celsius (°C)** and **Fahrenheit (°F)**.

---

## 🛠️ Key Technologies

| Category          | Used Technology        |
|------------------|------------------------|
| Framework        | Flutter (Dart)         |
| State Management | Provider               |
| Networking       | http package           |
| Local Storage    | SharedPreferences      |
| API              | OpenWeatherMap         |

---

## ✨ Features

### 🔍 Search Functionality
Search for weather conditions by city name using the OpenWeather API.

### 📊 Detailed Weather Data
- Real-time weather
- Temperature + Feels Like
- Weather icon and description
- Humidity, Pressure
- Wind speed
- Sunrise & Sunset times (converted to local time)

### ❤️ Favorites System
Save cities to a **Favorites List** (persisted locally using SharedPreferences).

### ⚙️ Settings Page
Toggle between:
- **Metric (°C)**
- **Imperial (°F)**

### ⚡ Error Handling
- Invalid city message
- Network issues handling
- Friendly UI messages

### 🔄 Loading States
Modern loading indicators while fetching data.

---

## 🛠️ Setup Steps

Follow the steps below to run the application:

### 1. Clone Repository

```bash
git clone https://github.com/your-username/weather-app.git
cd weather-app
````

### 2. Install Dependencies

```bash
flutter pub get
```

### 3. Run the App

Connect your device or open an emulator:

```bash
flutter run
```

---

## 🔑 API Usage & Configuration

This project uses the **OpenWeatherMap Current Weather API**.

### API Key Setup

The API Key is stored in a configuration file:

**File:** `lib/config/api_constants.dart`

```dart
class ApiConstants {
  static const String baseUrl =
      "https://api.openweathermap.org/data/2.5/weather";

  // ⚠️ Only for learning purposes – do not commit keys in real apps
  static const String apiKey = "YOUR_API_KEY";
}
```

### Example API URL

```
https://api.openweathermap.org/data/2.5/weather?q={CITY_NAME}&appid={API_KEY}&units={metric/imperial}
```

---

## 📂 Project Structure

Clean folder structure to separate concerns:

```
lib/
├── config/              # Configuration files (API constants)
├── models/              # Data models (WeatherModel)
├── pages/               # UI Screens
│   ├── home_page.dart
│   ├── details_page.dart
│   ├── favorites_page.dart
│   └── settings_page.dart
├── providers/           # State logic (WeatherProvider)
├── services/            # API service (WeatherService)
└── main.dart            # App entry point
```

---



## 📝 Assignment Requirements Checklist

* [x] Multi-page application
* [x] Fetch data from OpenWeatherMap API
* [x] Display temperature, humidity, wind, icon, etc.
* [x] Search by city name
* [x] Favorites using SharedPreferences
* [x] Settings toggle °C / °F
* [x] Error handling & loading states
* [x] State management with Provider
* [x] Clean code & folder structure

---

## 🎓 Developed For

**Assignment 3**
Mobile Application Development Course

---

## 👨‍💻 Author

Developed by **[Mostafaaa Hussein  Abdelal]**
Feel free to ⭐ the repository and contribute!

```
