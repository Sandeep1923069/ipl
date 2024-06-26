🔍 Project Overview:
- Title: IPL Data Analysis
- Objective: Utilizing the last 3 years of IPL data to identify the Best Team, top Batsman, Bowler, All-Rounder, Orange Cap and Purple Cap contenders, and predicting the teams with the highest chances of qualification in IPL 2024.

- Tools Used: Power BI Desktop, Microsoft Excel,SQL

📈 Key Insights:

🏆 Top Teams by Winning Percentage:
 1. GT - 70%
 2. LSG - 59%
 3. CSK - 56%
 4. RCB - 56%

🏏 Top 3 Batsmen by Runs:
 1. Shubman Gill - 1851 runs
 2. Faf du Plessis - 1831 runs
 3. Ruturaj Gaikwad - 1593 runs

🎯 Top 3 Bowlers by Wickets:
 1. Mohammad Shami - 67 wickets
 2. Yuzvendra Chahal - 66 wickets 
 3. Harshal Patel - 65 wickets

🌟 Top 3 All-Rounders (Minimum 500 runs and 25 wickets):
 1. Andre Russell - 745 runs, 35 wickets
 2. Ravindra Jadeja - 533 runs, 37 wickets
 3. Axar Patel - 505 runs, 30 wickets

💥 Top 3 Hitters (Minimum Balls Played 200):
 1. Tim David - 178 Strike Rate
 2. Heinrich Klaasen - 177 Strike Rate
 3. Liam Livingstone - 168 Strike Rate

🏏 Best Playing 11 based on last three years Data:
 1. Faf du Plessis
 2. Shubman Gill
 3. Suryakumar Yadav
 4. Glenn Maxwell
 5. Sanju Samson (WK) (c)
 6. David Miller
 7. Axar Patel
 8. Rashid Khan
 9. Jasprit Bumrah
 10. Mohammed Shami
 11. Yuzvendra Chahal

🔮 Predictions for IPL 2024:
 - Top 2 Orange Cap Contenders: Yashasvi Jaiswal, Shubman Gill
 - Top 2 Purple Cap Contenders: yuzvendra chahal, Arshdeep Singh
 - Top 4 Teams to Qualify: CSK, MI, LSG, GT/RCB





--------------------------------------------------------------------------------------------------------------------------------------------------------------
Project Overview


 Analyze the last 3 years of IPL data to find the best teams, batsmen, bowlers, all-rounders, top contenders for Orange Cap and Purple Cap, and teams with the highest chance of qualification.

Meta data- The document contains all the meta information regarding the columns described in the CSV files for a comprehensive analysis of IPL matches over the past three years (2021, 2022, 2023). I have provided 4 CSV files:

1. dim_match_summary
2. fact_batting_summary
3. fact_bowling_summary
4. dim_players





Column Description for dim_match_summary:
- team1: Name of the team batting first.
- team2: Name of the team batting second.
- winner: The team that won the match.
- margin: The margin by which the winning team won (runs or wickets).
- matchDate: The date on which the match was played, formatted as MMM DD, YYYY.
- match_id: Unique identifier for each match, prefixed with 'T'.

*******************************************



Column Description for dim_players:
- name: The full name of the player.
- team: The IPL team the player is associated with.
- battingStyle: The batting style of the player (e.g., Right hand Bat, Left hand Bat).
- bowlingStyle: The bowling style of the player (e.g., Right arm Offbreak, Legbreak).
- playingRole: The primary role of the player in the team (e.g., Batter, Bowler, Allrounder).



*******************************************



Column Description for fact_batting_summary:

match_id: Links to the dim_match_summary for match details, prefixed with 'T'.
match: Description of the match in "Team1 Vs Team2" format.
teamInnings: The team that is batting in the specified innings.
battingPos: The batting order position of the player.
batsmanName: The name of the batsman.
out/not_out: Indicates whether the batsman was out or not out.
runs: The number of runs scored by the batsman.
balls: The number of balls faced by the batsman.
4s: The number of boundaries (4 runs) hit by the batsman.
6s: The number of sixes hit by the batsman.
SR (Strike Rate): The strike rate of the batsman during the innings.


*******************************************




Column Description for fact_bowling_summary:

match_id: Links to the dim_match_summary for match details, prefixed with 'T'.
match: Description of the match in "Team1 Vs Team2" format.
bowlingTeam: The team that is bowling in the specified innings.
bowlerName: The name of the bowler.
overs: The number of overs bowled by the player.
maiden: The number of maiden overs bowled.
runs: The number of runs conceded by the bowler.
wickets: The number of wickets taken by the bowler.
economy: The bowler's economy rate.
0s: The number of dot balls bowled.
4s: The number of boundaries conceded.
6s: The number of sixes conceded.
wides: The number of wide balls bowled.
noBalls: The number of no balls bowled.





*******************************************
