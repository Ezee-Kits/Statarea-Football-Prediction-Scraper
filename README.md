# Statarea Football Prediction Scraper

This project automates the extraction of football match predictions from **Statarea.com** using **Requests** and **BeautifulSoup**.  
It gathers data such as **1X2**, **Over/Under 2.5**, and **Both Teams to Score (BTS/OTS)** percentages for the current or next match day, formats it into a structured dataset, and saves it as a CSV file for analysis.

---

## 🚀 Features
- Automatically scrapes football prediction data from Statarea.
- Extracts:
  - **Date** and **Time** of each match
  - **Home/Away Teams**
  - **Win/Draw/Away percentages**
  - **Over/Under 2.5 goals**
  - **Both Teams to Score (BTS/OTS)**
- Cleans, structures, and saves the data as a **CSV file**.
- Option to collect **today’s** or **tomorrow’s** matches automatically.

---

## ⚙️ Setup

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/statarea-data-scraper.git
cd statarea-data-scraper
2. Install dependencies
pip install requests beautifulsoup4

3. Project structure
statarea-data-scraper/
│
├── func.py
├── statarea.py
└── README.md


Note: The func.py file should include helper functions like
save_daily_csv, saving_files, and match_day_date.

▶️ Usage

Run the script:

python statarea.py


The program will:

Check if match_day_date equals 1 (to fetch tomorrow’s matches) or 0 (for today’s matches).

Scrape match data and predictions from Statarea.

Save the combined data into a CSV file named statarea.csv inside a dated folder.

📊 Output Example

Example of saved statarea.csv:

DATE,TIME,HOME TEAM,AWAY TEAM,HOME PER,DRAW PER,AWAY PER,UNDER 2.5,OVER 2.5,BTS,OTS,NAME
2025-10-19,15:00,Manchester United,Liverpool,48,25,27,42,58,51,49,STA
2025-10-19,18:00,AC Milan,Inter Milan,45,28,27,40,60,47,53,STA

💡 Example Use Case

You can use this script for:

Building a football prediction dashboard.

Combining data from multiple sources (Forebet, Prematips, Statarea, etc.).

Training machine learning models for football match outcome prediction.

Tracking accuracy trends of prediction websites over time.

🧰 Tech Stack

Python 3

Requests – for fetching webpage content.

BeautifulSoup4 – for parsing HTML and extracting data.

Datetime – for managing match dates.

Custom functions (in func.py) – for saving and managing files.

👨‍💻 Author

Ezee Kits
Focused on automation, data collection, and Python programming for predictive analytics.
📺 YouTube: Ezee Kits

📄 License

This project is licensed under the MIT License — you can freely use, modify, and share it with proper credit.
