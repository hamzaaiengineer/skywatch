# SkyWatch – Global Weather Desktop App
### Final Year Project | Electron + Open-Meteo API

---

## 📋 Project Overview

**SkyWatch** is a fully functional desktop weather application built with:
- **Electron.js** – Cross-platform desktop framework (Windows, macOS, Linux)
- **Open-Meteo API** – Free weather API (no key required)
- **Open-Meteo Geocoding API** – City search (no key required)
- **Chart.js** – Interactive forecast charts

---

## ✨ Features

| Feature | Description |
|---|---|
| 🔍 City Search | Search any city worldwide with live autocomplete |
| 🌡️ Current Weather | Temperature, feels like, weather condition |
| 💧 Stats Grid | Humidity, wind speed, precipitation, visibility |
| ⏰ 24-Hour Forecast | Scrollable hourly strip with icons |
| 📈 48-Hour Chart | Dual-axis temperature & humidity chart |
| 📅 7-Day Outlook | Daily forecast with high/low temps |
| ☀️ Sun & UV Info | Sunrise/sunset times, UV index, wind direction |
| ⭐ Save Cities | Bookmark cities for quick access (persisted) |
| 🌍 12 Quick Cities | One-click access to major world cities |
| 🖥️ Native Desktop | Custom titlebar, frameless window |

---

## 🚀 How to Run

### Prerequisites
- **Node.js** (v18 or later) — https://nodejs.org

### Steps

```bash
# 1. Clone or extract this project folder

# 2. Install dependencies
npm install

# 3. Run the app
npm start
```

That's it! The app will open as a native desktop window.

---

## 📦 Build Executable (Optional)

To create a distributable installer:

```bash
# Windows (.exe installer)
npm run build-win

# macOS (.dmg)
npm run build-mac

# Linux (.AppImage)
npm run build-linux
```

Output will be in the `dist/` folder.

---

## 🌐 APIs Used (All Free, No Key Needed)

### 1. Open-Meteo Forecast API
```
https://api.open-meteo.com/v1/forecast
```
Parameters used:
- `current`: temperature, humidity, apparent_temperature, precipitation, weather_code, wind_speed, wind_direction, visibility
- `hourly`: temperature, humidity, wind_speed, weather_code, precipitation_probability
- `daily`: weather_code, temp_max, temp_min, precipitation_sum, sunrise, sunset, uv_index_max

### 2. Open-Meteo Geocoding API
```
https://geocoding-api.open-meteo.com/v1/search
```
Used for city search autocomplete with country info.

---

## 🗂️ Project Structure

```
weather-app/
├── main.js          ← Electron main process (creates window)
├── index.html       ← Full app (HTML + CSS + JS in one file)
├── package.json     ← Dependencies and build config
└── README.md        ← This file
```

---

## 🎨 Design

- **Theme**: Dark, space-inspired with neon accent colors
- **Typography**: Syne (display) + DM Mono (data/numbers)
- **Color Palette**: Deep navy background, cyan/green accent, blue secondary

---

## 🔧 Technologies

| Tech | Version | Purpose |
|---|---|---|
| Electron | ^28 | Desktop window & native OS integration |
| Chart.js | 4.4.0 | Temperature & humidity forecast chart |
| Open-Meteo | Free | Weather data (no key needed) |
| HTML/CSS/JS | Vanilla | UI, animations, logic |

---

## 👨‍💻 Author

Your Name  
Final Year Project – [Your University Name]  
[Year]
