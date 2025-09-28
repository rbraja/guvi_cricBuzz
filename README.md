CRICBUZZ_DASHBOARD

A Streamlit-based Cricket Dashboard that consolidates live scores, player statistics, SQL analytics, and CRUD operations using a local cricket database and Cricbuzz API.

🚀 Features

📡 Live Scores – Fetch real-time cricket match updates.

👤 Player Stats – Search players and view detailed career statistics.

📊 SQL Analytics – Run SQL queries on cricket database for insights.

📝 CRUD Operations – Manage players, matches, venues, and series in the database.

📂 Project Structure
CRICBUZZ_DASHBOARD/
│── app.py                      # Main Streamlit app
│── cricket.db                  # SQLite database
│── modules/
│    ├── crud_ops.py            # CRUD operations page
│    ├── live_scores.py         # Live scores page
│    ├── player_stats.py        # Player statistics page
│    └── sql_analytics.py       # SQL analytics page
│── services/
│    ├── cricbuzz_api.py        # API integration (Cricbuzz RapidAPI)
│    └── db.py                  # Database connection and helper functions
│── .vscode/
│    └── launch.json            # VSCode debugging config
│── README.md                   # Project documentation

⚙️ Installation


Install dependencies

pip install streamlit pandas requests sqlite3


Run the app

streamlit run app.py

🔑 API Configuration

Update your Cricbuzz RapidAPI key in services/cricbuzz_api.py:

API_KEY = "your-rapidapi-key"

📊 Example SQL Queries

Find all players representing India.

Show matches played in the last few days.

Top 10 run-scorers.

Batting strike rates by year.

Venue-wise match statistics.
