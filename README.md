
# 🌦 MK Weather App: Discover & Forecast

A feature-rich **VB.NET desktop application** that provides real-time weather information and 5-day forecasts using the OpenWeatherMap API.

## 🚀 Features
- 🔐 User Login & Signup (MS Access backend)
- 🌍 Live Current Weather Search by City
- 📆 5-Day Weather Forecast using JSON API
- 🕒 Auto-load Last Searched City on Launch
- 📜 Search History (View, Delete, Clear All)
- ❤️ Favorite Cities:
  - Save, View, Delete Favorites
  - Auto-suggest Favorites near input
- 🎨 Beautiful WinForms UI with VB.NET
- 🔒 ADO.NET based secure data access

## 🛠 Technologies Used
- **VB.NET (Visual Studio 2022)**
- **ADO.NET**
- **Microsoft Access 2016**
- **OpenWeatherMap API**
- **WinForms**

## 🗄 Database Tables
- `Users` – Stores login credentials
- `SearchHistory` – Stores each user's search history
- `FavoriteCities` – Stores user’s favorite cities


## 📁 Folder Structure
```
WeatherApp/
│
├── Forms/
│   ├── LoginForm.vb
│   ├── SignupForm.vb
│   ├── Form1.vb (Main)
│   ├── HistoryForm.vb
│   └── FavoriteCityForm.vb
├── AboutForm.vb
├── WeatherApp.accdb (Access DB)
└── README.md
```

## 🧑‍💻 How to Run This Project on Another Laptop

### Requirements
- Windows 7 or later
- .NET Framework 4.5 or higher
- Visual Studio 2022 (Community Edition recommended)
- MS Access 2016 or later (for `.accdb` support)

### Setup Instructions

1. **Clone or download the repository:**

```bash
git clone https://github.com/Mohit7172/MK-Weather-App.git
```

2. **Open the project in Visual Studio:**

- Open Visual Studio 2022
- Select **Open a local folder** and choose the `WeatherApp` folder

3. **Place the Database File:**

Copy `WeatherApp.accdb` from the project folder to your Documents folder:

```
C:\Users\YOURNAME\Documents\WeatherApp.accdb
```

4. **Update Connection Strings (if needed):**

In the VB.NET code files (e.g. `Form1.vb`, `LoginForm.vb`), update the database path in connection strings like this:

```vb
"Provider=Microsoft.ACE.OLEDB.12.0;Data Source=C:\Users\YOURNAME\Documents\WeatherApp.accdb;"
```

5. **Install Newtonsoft.Json Package:**

- In Visual Studio, go to **Tools > NuGet Package Manager > Manage NuGet Packages for Solution**
- Search for `Newtonsoft.Json` and install the latest stable version

6. **Add your OpenWeatherMap API Key:**

- Open `App.config`
- Replace the placeholder with your API key:

```xml
<add key="WeatherApiKey" value="YOUR_API_KEY_HERE" />
```

### Run the Project

Press `F5` or click the **Start** button in Visual Studio to build and run the application.

---

## 👨‍💻 Developed By
- **Mohit Kumar**


## 🔗 Useful Links
- [OpenWeatherMap](https://openweathermap.org/)
- [VB.NET Documentation](https://learn.microsoft.com/en-us/dotnet/visual-basic/)

## 📃 License
This project is for educational and demonstration purposes only.
