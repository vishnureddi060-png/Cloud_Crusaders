Atmospheric Analysis Console
A futuristic, sci-fi themed web interface for visualizing simulated atmospheric data. This standalone application uses Leaflet.js for interactive map controls and Chart.js for dynamic data visualization, all wrapped in a custom-styled, responsive UI.

▶️ View Live Demo (Link)
Features
Interactive Map Interface: Select any location on the globe using an interactive map powered by Leaflet.

Location Search: Use the geocoder to search for specific target locations by name.

Click-to-Select: Click directly on the map to update the target coordinates and automatically fetch the location's name.

Simulated Analysis: Initiates a mock analysis process that simulates fetching and processing atmospheric data (Aerosol Optical Depth, NO₂) to predict PM2.5 levels.

Dynamic Data Visualization: Displays a 10-day PM2.5 forecast in an animated line chart using Chart.js.

Key Metrics Display: Shows critical metrics like Peak PM2.5, 10-Day Average, and the number of days with anomalous readings.

Threat Alert System: Automatically generates and displays color-coded alerts for days with elevated or critical pollution levels.

Fully Responsive Design: The UI seamlessly transitions from a desktop side-panel layout to a mobile-friendly stacked layout.

Thematic UI/UX: A custom, futuristic "hacker" aesthetic is achieved with pure CSS, including custom fonts, glow effects, animated loaders, and unique panel shapes.

How To Use
Open the Application: Simply open the index.html file in any modern web browser.

Select a Location:

Click and drag the map to pan.

Use the search bar in the top left to find a location by name.

Click anywhere on the map to set that point as the analysis target.

Run Analysis: Click the "INITIATE ANALYSIS" button in the control panel.

View Results: The dashboard will display the 10-day prediction chart, key metrics, and any relevant threat alerts for the selected location.

Technology Stack
This project is built as a single, self-contained HTML file and leverages powerful open-source libraries.

Frontend: HTML5, CSS3, JavaScript (ES6+)

Mapping: Leaflet.js for the interactive map and markers.

Map Tiles: CartoDB high-contrast dark matter tiles.

Geocoding: Leaflet Control Geocoder with Nominatim for location search.

Charting: Chart.js for beautiful and responsive data visualizations.

Fonts: Google Fonts (Orbitron for displays, Roboto Mono for text).

Code Overview
index.html: Contains the complete structure, styling, and logic.

CSS: All styling is within the <style> tags. It uses CSS Custom Properties (variables) for easy theme management (colors, fonts). Advanced techniques like clip-path and @keyframes animations are used to achieve the futuristic aesthetic.

JavaScript: The entire application logic is within the <script> tags.

State Management: A global selectedRegion object tracks the user's target.

Map Initialization: Sets up the Leaflet map, tile layers, geocoder, and custom marker icon.

Event Handlers: Listens for map clicks and button clicks to trigger analysis.

Simulated Backend (runCloudAnalysis): An async function that mimics an API call, generating mock data and predictions to drive the UI.

UI Update Functions: A set of functions (displayChart, displayMetrics, displayAlerts) are responsible for rendering the analysis results dynamically.

Setup
No setup is required. Simply download the index.html file and open it in a web browser. All external libraries (Leaflet, Chart.js) are loaded via CDN.

License
This project is licensed under the MIT License. See the LICENSE file for details.
