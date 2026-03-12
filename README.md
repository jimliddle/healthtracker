🩺 Personal Health Tracker

A privacy-first, fully responsive, and offline-capable single-page application (SPA) for tracking your essential health metrics. Log your blood pressure, heart rate, and weight, visualize your trends over time, and easily import historical data from Withings.

Because this app uses your browser's native IndexedDB, all your health data remains completely private and is stored locally on your device. No cloud, no tracking, no backend required.

<img width="915" height="510" alt="health tracker screenshot" src="https://github.com/user-attachments/assets/04cab9e6-d72e-4bc8-a4f5-6c6dfb3c2c89" />


✨ Features

Comprehensive Logging: Record Blood Pressure (Systolic/Diastolic), Heart Rate (BPM), and Weight (kg) with date and time stamps.

- Interactive Dashboards: View your data filtered by:

- Past Week

- Past Month

- Year to Date (YTD)

- All Time

- Automatic Statistics: Calculates averages, highs, and lows for the selected time period automatically.

- Visual Charts: Beautiful, interactive line graphs built with Chart.js to help you visualize your health trends at a glance.

- Withings Data Import: Seamlessly import your historical health data via CSV exports from the Withings Health app. The app intelligently merges new metrics without overwriting your existing local data.

- Data Management: View a detailed history table, delete individual errant entries, or completely wipe your local database if needed.

- Responsive Design: Built with Tailwind CSS, ensuring a perfect, app-like experience on both desktop and mobile browsers.

🛠️ Tech Stack

This project is built using vanilla HTML, CSS, and JavaScript, relying on powerful CDN-delivered libraries to keep the footprint ultra-lightweight:

- Tailwind CSS - For responsive, utility-first styling.

- Dexie.js - A minimalist wrapper for IndexedDB, making local browser storage reliable and easy to query.

- Chart.js - For rendering smooth, interactive HTML5 canvas charts.

- PapaParse - For lightning-fast, robust CSV parsing (used for the Withings import feature).

- FontAwesome - For crisp, scalable vector icons.

🚀 Getting Started

Since there is no backend or build step required, running the app is incredibly simple.

Simply download the webpage and double click to load or visit the hosted version (all state stored in your browser):

https://jimliddle.github.io/healthtracker/


📥 Importing Withings Data

If you are transitioning from or syncing with Withings products (like smart scales or blood pressure monitors):

- Go to your Withings web dashboard and request a data export.

- Download the resulting .zip file and extract it.

- Locate the .csv file containing your measurement data (often named raw_tracker_measures.csv or similar).

- Open the Health Tracker App, click Import Withings in the top navigation bar, and select your CSV file.

- The app will automatically parse the dates, times, weights, heart rates, and blood pressures and append them to your local database.

🛡️ Privacy & Security

This application is strictly client-side.

It does not connect to any external databases.

It does not send telemetry or analytics.

If you clear your browser data (or use the "Clear All" button in the app), your data is permanently deleted. If you want to back up your data, do not clear your browser cache without a backup strategy.

🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

📝 License

This project is MIT licensed.
