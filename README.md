-----

# Atmospheric Analysis Console

*A sleek, sci-fi themed dashboard for visualizing simulated atmospheric data.*

-----

This standalone web application provides a futuristic interface for monitoring simulated atmospheric conditions. It uses **Leaflet.js** for interactive map controls and **Chart.js** for dynamic data visualization, all wrapped in a custom-styled, responsive UI.

### [▶️ View Live Demo](https://www.google.com/search?q=https://your-demo-link-here.com)

-----

## ✨ Features

  * 🗺️ **Interactive Map Interface**: Select any location on the globe using a smooth, interactive map powered by Leaflet.
  * 🔍 **Location Search & Geocoding**: Use the built-in geocoder to search for specific target locations by name.
  * 🖱️ **Click-to-Select**: Instantly update the target coordinates by clicking directly on the map, with automatic location name resolution.
  * 🛰️ **Simulated Analysis**: Initiate a mock backend process that simulates fetching and processing atmospheric data (Aerosol Optical Depth, NO₂) to predict PM2.5 levels.
  * 📊 **Dynamic Data Visualization**: View a 10-day PM2.5 forecast in an animated, gradient-filled line chart using Chart.js.
  * 📈 **Key Metrics Display**: At a glance, see critical metrics like **Peak PM2.5**, **10-Day Average**, and the number of **Anomalous Days**.
  * 🚨 **Threat Alert System**: Automatically generates and displays color-coded alerts for days with "Elevated" or "Critical" pollution levels.
  * 📱 **Fully Responsive Design**: The UI seamlessly transitions from a desktop side-panel layout to a mobile-friendly stacked view.
  * 👽 **Thematic UI/UX**: A custom, futuristic "hacker" aesthetic is achieved with pure CSS, including custom fonts, glow effects, animated loaders, and unique `clip-path` panel shapes.

-----

## 🛠️ Technology Stack

This project is built as a single, self-contained HTML file and leverages powerful open-source libraries.

  * **Core**: HTML5, CSS3, and modern JavaScript (ES6+).
  * **Mapping**: **[Leaflet.js](https://leafletjs.com/)** for the interactive and responsive mapping interface.
  * **Charting**: **[Chart.js](https://www.chartjs.org/)** for beautiful and animated data visualizations.
  * **Map Tiles**: High-contrast dark matter tiles from **[CartoDB](https://carto.com/)**.
  * **Geocoding**: **[Leaflet Control Geocoder](https://github.com/perliedman/leaflet-control-geocoder)** utilizing the **[Nominatim](https://www.google.com/search?q=https://nominatim.openstreetmap.org/)** service.
  * **Fonts**: **[Google Fonts](https://fonts.google.com/)** (`Orbitron` for displays and `Roboto Mono` for text).

-----

## 🚀 How to Use

1.  **Download**: Get the `index.html` file.
2.  **Open in Browser**: Open the file in any modern web browser (e.g., Chrome, Firefox, Edge).
3.  **Select a Target**: Use the search bar or click directly on the map to choose a location.
4.  **Initiate Analysis**: Click the **"INITIATE ANALYSIS"** button.
5.  **Review the Data**: Observe the generated chart, metrics, and alerts in the dashboard.

-----

## 📂 Code Structure

The entire project is encapsulated within a single `index.html` file for ultimate portability.

  * **CSS**: All styling is located within the `<style>` tags.
      * It uses **CSS Custom Properties** (variables) for easy theme management.
      * Advanced techniques like `clip-path` and `@keyframes` animations create the futuristic aesthetic.
  * **JavaScript**: All application logic is within the `<script>` tags.
      * **State Management**: A global `selectedRegion` object tracks the user's target.
      * **Map Initialization**: Sets up the Leaflet map, tile layers, geocoder, and custom marker.
      * **Event Handlers**: Listens for map and button clicks to trigger analysis.
      * **Simulated Backend**: The `runCloudAnalysis()` async function mimics an API call, generating mock data and predictions to drive the UI.
      * **UI Update Functions**: A set of modular functions (`displayChart`, `displayMetrics`, `displayAlerts`) are responsible for rendering the analysis results.

-----

## 📦 Installation

**No installation is required.** Simply download the `index.html` file and open it locally in your web browser. All external libraries are loaded via a CDN.

## 📄 License

This project is licensed under the **MIT License**.
