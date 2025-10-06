# 🌤️ Weather App - ASE Challenge Submission

A **modern, responsive, single-page weather application** built with **React, Tailwind CSS, TanStack Query, and shadcn/ui**. This app allows users to search for cities, view current weather and a 5-day forecast, manage favorites, and toggle dark mode.

---

##  Demo-Link

https://weathercheker.netlify.app/


<img width="1905" height="850" alt="image" src="https://github.com/user-attachments/assets/b9a9d307-2895-4d14-b8ab-0fb672531c29" />

#Light mode#

<img width="1887" height="860" alt="image" src="https://github.com/user-attachments/assets/5e92324c-a0d5-42bf-9376-1fa1faafc2dc" />


---

## ✨ Features

### Core Features
- 🔍 **Search Box**: Search for any city to fetch current weather data.
- 🌡 **Current Weather Display**: Shows temperature, humidity, and weather conditions.
- 📅 **5-Day Forecast**: View temperature and weather for the next 5 days.
- 🌗 **Dark Mode Toggle**: Switch between light and dark themes.
- ⭐ **Favorites Section**: Save your favorite cities for quick access.
- 💾 **LocalStorage Integration**: Persist search history and favorite cities across sessions.
- 🔄 **Refresh Button**: Reload the weather data for a city.
- 🗺️ **City Details Page**: Navigate to a dedicated page for more detailed weather information.

---

## 🛠️ Tech Stack

- **Frontend:** React.js (Vite)  
- **Styling:** Tailwind CSS + shadcn/ui components  
- **State Management:** TanStack Query (React Query)  
- **API:** [OpenWeatherMap](https://openweathermap.org/api)  
- **Other:** LocalStorage for storing last searched cities and favorites  

---

## ⚡ Setup & Installation

### Prerequisites
- Node.js (v18+)
- npm or yarn

### Steps

1.  **Clone the repository:**
    ```bash
    git clone 
    cd weather-app
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    # or
    yarn install
    ```
3.  **Configure API Key:**
    Create a `.env` file in the root directory and add your OpenWeatherMap API key:
    ```
    VITE_WEATHER_API_KEY=your_api_key_here
    ```
4.  **Start the development server:**
    ```bash
    npm run dev
    # or
    yarn dev
    ```
5.  Open `http://localhost:5173` in your browser.

---

## ⚙️ How It Works

### Search & Data Flow
1.  Users type a city name into the search box.
2.  This input triggers a data fetch using **TanStack Query**.
3.  The application uses the city name to fetch current weather and a 5-day forecast from the **OpenWeatherMap API**.
4.  Data is then displayed in the Current Weather and 5-Day Forecast components.

### Persistence
-   The last searched cities and user-defined favorite cities are managed and stored in the browser's **LocalStorage**, ensuring data remains available even after the user closes and reopens the app.

### Navigation
-   Clicking on a saved city or the currently searched city allows navigation to a dedicated **City Details Page** for a richer view of the weather data.

---

## 🎨 Design & UX Choices
-   **Mobile-First, Responsive Design:** All components are designed to adapt seamlessly from mobile screens up to large desktop displays.
-   **Clean UI:** Utilizes **Tailwind CSS** and **shadcn/ui** for a modern, minimalist, and accessible user interface.
-   **Robust Feedback:** Implements proper loading states (skeletons during API calls) and user-friendly error messages to provide a clear experience.
