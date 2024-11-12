# GreatestEPLManager
Data collection to answer who is the greatest English Premier League manager

The Invincibles. The Centurions. The Mighty Red Devils. The English Premier League has witnessed to number of great teams, teams whose names would forever go down in history. A lot can be said about how individuals can light up a game but to win the league, you’d have to do it consistently across 20 plus games. That’s why I believe for a team to truly be great and leave its mark on this fantastic league, it needs an all-team effort. This includes the staff. And this analysis will focus on the people who call the shots, you have their teams playing a certain style, who hold the players accountable and motivate them to perform week in, week out. I’m talking about the managers/head coaches. You have probably heard of the names Sir Alex Ferguson, Arsene Wenger, Jose Mourinho, Pep Guardiola. These men have set their names apart from their peers by hauling in multiple trophies, giving talented players the right platform to shine and helping build a massive global fanbase in their respective clubs. 
English football has been going for a long time, its origins trace back to days before my country got its independence. Back then, stat compiling and records were not as prevalent as they are now. So, this analysis will begin from the 1992/1993 season as the English Premier League as we know it was founded as the FA Premier League on 20 February 1992, following the decision of First Division (the top-tier league from 1888 until 1992) clubs to break away from the English Football League. The analysis will also end in the 2023/2024.

•	Steps:
•	The data was collected via web scraping from the Transfermarkt site and the Premier League official website.
•	I knew I’d need 3 main datasets. One for the all the end of season league tables. Another dataset for the manager history (e.g. containing their appointed date, win ratio, matches coached, matches lost etc.) And lastly, a dataset for all the matches played in the range of my analysis (1992/93 to 2023/24)
•	First, to get a whole list of teams that had played in the EPL. I collected data from the premier league site. Then using the team names, I was able to create team ids for all the teams. Then collected the league tables for all the seasons to be analyzed from Transfermarkt. After this was done, I collected the manager table from Transfermarkt. I also created a manager ID by using characters from the manager’s name and the team id of the teams they managed. For Example, Jose Mourinho would have three manager ids for his time at Chelsea, Manchester United and Tottenham. Then I mapped each manager id to a home and away team in the matches dataset to indicate which manager was appointed for each game for the range of my analysis.

![all_matches_test ipynb - datacleaning - Visual Studio Code  Administrator  01_10_2024 17_53_15](https://github.com/user-attachments/assets/7274c425-44dc-4c36-9d48-f14cad61ab99)


Tools used:
VS Code, Python, Selenium, Pandas, BeautifulSoup

