🏀 NBA Team Stats Analyzer
My First Python Data Project

A beginner-friendly script that combines and cleans NBA data for analysis

🌟 About This Project
This was my first Python data project where I learned to:

Load and explore CSV files using pandas

Combine datasets with SQL-like joins (thanks to pandasql!)

Handle missing data by filling arena capacities

Transform columns (splitting home records into wins/losses)

Prepare data for Power BI visualization

The script takes raw NBA team stats and franchise info, cleans them up, and outputs analysis-ready data.

🛠️ How It Works
Data Processing Steps:
Input Files

ranking.csv: Team performance (wins, losses, home records)

teams.csv: Franchise details (location, arena, management)

Magic Happens

Merges datasets to connect teams with their stats

Fixes missing arena capacities using average values

Splits "24-7" home records into separate win/loss columns

Output
Clean nba_clean.csv ready for Power BI dashboards

🚀 Getting Started
Prerequisites

bash
Copy
pip install pandas pandasql
Run the Script

bash
Copy
python nba_analysis.py
Visualize
Import nba_clean.csv into Power BI to create your first dashboard!

📊 Sample Analysis Ideas
Which teams have the best home records?

Does arena capacity correlate with team success?

Compare conference performance

💡 Lessons Learned
Through this project I:

Discovered how real-world data often needs cleaning

Learned to troubleshoot errors (like column name mismatches!)

Gained confidence working with Python and datasets

🤝 Want to Improve This?
Suggestions welcome! This is my first project and I'm excited to keep learning.

"The first of many data projects!"

This version:
✅ Keeps it beginner-friendly but professional
✅ Highlights your learning journey
✅ Explains the technical process simply
✅ Includes motivational elements
✅ Maintains clean formatting

Want to add a screenshot of your final data? Or include your Power BI dashboard image later? Just paste it in!
