# AbuseMap - Punjab Incident Dashboard 

**Live Demo:** [https://abusemap-cc3h-141.onrender.com](https://abusemap-cc3h-141.onrender.com)

AbuseMap is a real-time, state-of-the-art dashboard designed to monitor and visualize animal cruelty and rescue incidents across the Punjab region of India. It combines automated news scraping with user-driven reporting to provide actionable insights for animal welfare.

## Features

- **Automated Intelligence**: An integrated scraper that scans Google News RSS feeds to find live animal cruelty/rescue reports.
- **Dynamic Heatmaps**: Visualizes high-risk zones using Leaflet.js with time-range filtering (7 Days, 30 Days, All Time).
- **Real-time Analytics**: Interactive charts (Trend Analysis and Incident Types) powered by Chart.js.
- **Advanced Search**: Instant, cross-field search for cities, incident types, and descriptions.
- **Incident Management**: A searchable log for admins to track and update the status of reports (Pending, Working, Resolved).
- **Premium UI**: A sleek, dark-themed dashboard using modern glassmorphism design principles.

## Technology Stack

### Backend
- **Node.js & Express**: API server and static file hosting.
- **SQLite**: Lightweight, persistent database for storing incident records.
- **RSS Parser**: For automated news gathering from Google News.

### Frontend
- **Leaflet.js**: Interactive maps and heatmaps.
- **Chart.js**: Data visualization and trend analysis.
- **Vanilla JavaScript & CSS3**: Custom logic and premium dark-mode styling.

## Project Structure

- `server.js`: Main Express server and API routes.
- `scraper.js`: Automated Google News scraper and data categorizer.
- `db.js`: SQLite database configuration.
- `index.html`: Dashboard structure and SPA navigation.
- `app.js`: Client-side logic for maps, charts, and API interaction.
- `styles.css`: Custom premium styling and design system.

## Setup & Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/PrabhSaran-07/Abusemap-CT-Hackathon-.git
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the server**:
   ```bash
   node server.js
   ```

4. **Access the dashboard**:
   Open your browser and navigate to `http://localhost:3000`.

## How It Works

1. **Data Collection**: On startup (and every hour), the backend scraper queries Google News for animal-related incidents in Punjab.
2. **Geocoding**: The system parses the news headlines to identify cities and assigns coordinates dynamically.
3. **API Bridge**: The frontend fetches this data via a REST API.
4. **Visualization**: Data is processed on the client side to update the Punjab Heatmap and Analytics charts.

---
Built for the **CT Hackathon**. Dedicated to improving animal welfare through technology.
