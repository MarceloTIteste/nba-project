# 🏀 NBA Team Stats Analyzer  
*A beginner Python project for sports data analysis*

![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=flat&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/power_bi-F2C811?style=flat&logo=powerbi&logoColor=black)

## 📖 About This Project
This was my first Python data project! I created a script that:
- Combines NBA team statistics with franchise information
- Cleans and prepares the data for analysis
- Outputs a Power BI-ready dataset

Through this project I learned to work with pandas, handle real-world data issues, and use SQL-like joins in Python.

## 🔧 How It Works

### Data Flow
1. **Input Files**:
   - `ranking.csv` - Team performance data (wins, losses, etc.)
   - `teams.csv` - Franchise information (locations, arenas, etc.)

2. **Processing**:
   ```python
   # Merge datasets
   query = """
       SELECT r.TEAM, t.ABBREVIATION, t.CITY, r.W, r.L, r.W_PCT, 
              r.HOME_RECORD, t.ARENACAPACITY
       FROM ranking_df r
       LEFT JOIN teams_df t ON r.TEAM_ID = t.TEAM_ID 
                            AND r.LEAGUE_ID = t.LEAGUE_ID
   """
   joined_df = sqldf(query, globals())
   
   # Clean data
   joined_df['ARENACAPACITY'] = joined_df['ARENACAPACITY'].fillna(arena_avg)
