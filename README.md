# GreatestEPLManager
Data collection to answer who is the greatest English Premier League manager.

The proper documentation is found in the word file provided in this repository.

The Invincibles. The Centurions. The Mighty Red Devils. The English Premier League has witnessed to number of great teams, teams whose names would forever go down in history. A lot can be said about how individuals can light up a game but to win the league, you’d have to do it consistently across 20 plus games. That’s why I believe for a team to truly be great and leave its mark on this fantastic league, it needs an all-team effort. This includes the staff. And this analysis will focus on the people who call the shots, you have their teams playing a certain style, who hold the players accountable and motivate them to perform week in, week out. I’m talking about the managers/head coaches. You have probably heard of the names Sir Alex Ferguson, Arsene Wenger, Jose Mourinho, Pep Guardiola. These men have set their names apart from their peers by hauling in multiple trophies, giving talented players the right platform to shine and helping build a massive global fanbase in their respective clubs. 
English football has been going for a long time, its origins trace back to days before my country got its independence. Back then, stat compiling and records were not as prevalent as they are now. So, this analysis will begin from the 1992/1993 season as the English Premier League as we know it was founded as the FA Premier League on 20 February 1992, following the decision of First Division (the top-tier league from 1888 until 1992) clubs to break away from the English Football League. The analysis will also end in the 2023/2024.

•	Steps:
•	The data was collected via web scraping from the Transfermarkt site and the Premier League official website.
•	I knew I’d need 3 main datasets. One for the all the end of season league tables. Another dataset for the manager history (e.g. containing their appointed date, win ratio, matches coached, matches lost etc.) And lastly, a dataset for all the matches played in the range of my analysis (1992/93 to 2023/24)
•	First, to get a whole list of teams that had played in the EPL. I collected data from the premier league site. Then using the team names, I was able to create team ids for all the teams. Then collected the league tables for all the seasons to be analyzed from Transfermarkt. After this was done, I collected the manager table from Transfermarkt. I also created a manager ID by using characters from the manager’s name and the team id of the teams they managed. For Example, Jose Mourinho would have three manager ids for his time at Chelsea, Manchester United and Tottenham. Then I mapped each manager id to a home and away team in the matches dataset to indicate which manager was appointed for each game for the range of my analysis.
•	I made sure to include only managers who had managed teams in the EPL during the range of analysis. So, names like Kieran McKenna are not included because he had not managed Ipswich Town during their time in the EPL until the 2024/2025 season.
•	For data cleaning, I mainly had to change the manager names to acceptable English format using unidecode. 


The datasets for this project were obtained through web scraping websites such as Transfermarkt and the official Premier League website. Python and several libraries were the tools used for the web scraping. This information is publicly available, in later sections I will show how the data was obtained. The data consists of three main tables:
•	All the league tables from the 1992/1993 season to the 2023/2024 season. Each league table for each season consists of 20 rows for each team and 10 columns for Table Position, Team Name, Number of Games Played, Number of Games Won, Number of Games Drawn, Number of Games Lost, Goals (Scored : Against), Goal Difference, Points Gained, Manager(s) In Charge of The Team over the Course of the season. (The League Tables for the 1992/1993 season to the 1995/1996 season have 22 rows). The league tables were later consolidated into one in Power BI adding a new column to indicate what season the league table was originally from.
•	The manager history table consists of 487 and 15 columns for Manager ID, Team ID, Team Name, Manager Name, Date Appointed, End of Time, Time in Post, Number of Matches Managed, Number of Games Won, Number of Games Drawn, Number of Games Lost, Points Per Game, Points Accumulated, Win Ratio, Seasons Managed.
•	The matches table consists of 11953 rows and 14 columns for Match ID, Match Day in Season, Date Match Was Played, Home Team, Home Team ID, Home Team Manager, Home Team Manager ID, Home Team Score, Away Team Score, Away Team, Away Team ID, Away Team Manager, Away Team Manager ID, Season Match Was Played.


![all_matches_test ipynb - datacleaning - Visual Studio Code  Administrator  01_10_2024 17_53_15](https://github.com/user-attachments/assets/7274c425-44dc-4c36-9d48-f14cad61ab99)


Tools used:
VS Code, Python, Selenium, Pandas, BeautifulSoup

