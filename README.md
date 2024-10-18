# PREDICT RESULTS OF 2023-24 NBA REGULAR SEASON GAMES WITH LOGISTIC REGRESSION BY OLUTOSIN FASHUSI
![logisticRegression20240222Results](https://github.com/user-attachments/assets/e998877d-bd8b-41d2-af2b-629f48ab66d9)
• Excerpt from NBA games played on 2024-02-22 predicted by model: miscStandardizedOddsRatio <br>
• miscStandardizedOddsRatio model has accuracy score of 74.4% correct for all games predicted compared to betting favorite <br>
• DATE: Model predictions begin on games played after 2024 All Star Game played on 2024-02-18 <br>
• GAMEID: Every NBA game has a unique GAMEID<br>
• MODEL PREDICTS: Abbreviation of team that model predicts to win <br>
• ACTUAL WINNER: (Abbreviation of team that actually won the game, ✅ if model vs actual winner model prediction correct ❌ if incorrect) <br>
• BETTING FAVORITE: (Abbreviation of team that started game as betting favorite, match spread, ✅ if model vs betting betting favorite model prediction correct ❌ if incorrect)
# TEST DETAILS
[comment]: ![testDetails](https://github.com/user-attachments/assets/72368df1-5cc2-43fd-b24e-af3786afb592)
![testDetails](https://github.com/user-attachments/assets/ae635e80-c5f9-420f-9a14-86b8888e5fa5)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested with feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: For every match, team with the larger probability estimate is predicted winner
# DECISION BOUNDRY PLOTS 
[comment]: ![ORL](https://github.com/user-attachments/assets/025fbd87-c001-4fc9-9f4f-540ad36deb15)
[comment]: ![CLE](https://github.com/user-attachments/assets/572ecdf7-3c48-4fbe-8bcd-03f54f637bd8)
![ORL](https://github.com/user-attachments/assets/aff57972-8b5a-45a9-b4fe-52bffa78d6d5)
![CLE](https://github.com/user-attachments/assets/6a7cef13-c2d5-4e2c-b419-3a2f078f4211)
![DET](https://github.com/user-attachments/assets/ec0d837d-84c7-4160-bf25-29ba34b5eb28)
![IND](https://github.com/user-attachments/assets/f2a69a8d-b60e-417a-b994-48ad5f5691c3)
![NYK](https://github.com/user-attachments/assets/256e3ff2-4df0-4d87-9708-81038949bdea)
![PHI](https://github.com/user-attachments/assets/3d6a6c5d-c8b6-432b-b98c-14b8b1b4b3a5)
![BKN](https://github.com/user-attachments/assets/f5a86c9b-cb95-465d-a07b-cf76d12c226a)
![TOR](https://github.com/user-attachments/assets/e01d3ce7-c268-440f-a25d-ea4d686f9407)
![PHX](https://github.com/user-attachments/assets/6e076d8f-638d-41c8-916a-7cf04a9cde21)
![DAL](https://github.com/user-attachments/assets/f5f3abee-92a3-4991-9a38-cbd550da6b7c)
![BOS](https://github.com/user-attachments/assets/63f971ac-9d02-42b1-9027-adfc0dcba238)
![CHI](https://github.com/user-attachments/assets/e6966a89-83be-42dc-ae4c-e93eec5164a5)
![HOU](https://github.com/user-attachments/assets/b69a4100-be18-4762-bc43-6b63404be897)
![NOP](https://github.com/user-attachments/assets/410051dc-66c3-4404-80a3-9c30840cd2bc)
![LAC](https://github.com/user-attachments/assets/0f6d1198-a43c-4e7f-8c1f-05ca21e9cfc9)
![OKC](https://github.com/user-attachments/assets/d2916eec-773f-4ea6-a6f2-10c963cd4f94)
![WAS](https://github.com/user-attachments/assets/7a14e75f-4837-4edf-9aca-ccee9df72171)
![DEN](https://github.com/user-attachments/assets/4fe1ef7a-f101-4b68-afb0-bf504b4b9cb0)
![CHA](https://github.com/user-attachments/assets/94649217-925c-4136-9ed6-d56708a7680d)
![UTA](https://github.com/user-attachments/assets/856f87f6-b76f-4751-9f75-d9019b19e61b)
![LAL](https://github.com/user-attachments/assets/5b12029e-e251-43e6-ac70-f0e0019c4e17)
![GSW](https://github.com/user-attachments/assets/3c6689ac-7ffb-4f65-bdba-c32136cca6dd)
![SAS](https://github.com/user-attachments/assets/a3b37c11-3169-482b-8031-faa611ffd9ce)
![SAC](https://github.com/user-attachments/assets/070f6730-32cd-4b5e-ab9e-60f1e2abb3ca)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Trained with previous feature values from [Misc Box Score](https://www.nba.com/stats/teams/boxscores-misc?SeasonType=Regular+Season&Season=2023-24) <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio, for example model identifies Fast Break Points in last game played (L1) as best feature for team: ORL (Orlando Magic) 
# OBJECTIVES:
•	For each of the 30 NBA teams, utilize data from previous games played to calculate probability estimate of team winning their next game <br>
•	Model predictions begin on games played post the NBA 2024 All Star Game (Feb. 28 2024) <br>
•	Compare model's predicted winner to 1) actual winner 2) betting favorite <br>
•	Identify features with greatest impact on team wins
# DATA SOURCES: 
<b><i>NBA.com</i></b><br>
&nbsp;&nbsp;&nbsp; [Traditional Box Score](https://www.nba.com/stats/teams/boxscores-traditional?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [Advanced Box Score](https://www.nba.com/stats/teams/boxscores-advanced?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [Four Factors  Box Score](https://www.nba.com/stats/teams/boxscores-four-factors?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [Misc Box Score](https://www.nba.com/stats/teams/boxscores-misc?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [Scoring Box Score](https://www.nba.com/stats/teams/boxscores-scoring?SeasonType=Regular+Season&Season=2023-24) <br>
&nbsp;&nbsp;&nbsp; [NBA Stats Glossary](https://www.nba.com/stats/help/glossary) <br>
<br>
<b>VEGASINSIDER.com</b> <br>
&nbsp;&nbsp;&nbsp; [NBA Odds & Betting Lines](https://www.vegasinsider.com/nba/odds/las-vegas)
# CONCLUSIONS:
<b>PREDICTION RESULTS BY TEAM</b>
<br>
![percentCorrect](https://github.com/user-attachments/assets/f4bd464f-4f98-4a1a-99c6-d4528ec3c47e)
<b><i> Gaps exists because model makes 0 predictions of a Pistons win </i></b>
<br><br>
![numberCorrect](https://github.com/user-attachments/assets/d87384fe-95e5-4797-b5c8-fccc0a5adf93)
<b><i> Model correclty predicts a league high of 26 vs Actual Result & 21 vs Betting Favorite for Boston Celltics </i></b>
<br><br>
![numberincorrect](https://github.com/user-attachments/assets/bdccbdce-02f5-4cd5-bfa6-cf3c6e9b565e)
<b><i> Model incorrectly predicts a league high of 12 vs Actual Result for Cleveland Cavaliers </i></b>
<br>
# CONCLUSIONS:
<b>FEATURE IMPACT BY TEAM</b><br>
<i>Teams where same feature is used for all team predictions are highlighted</i>
<br><br>
![maxFeatures](https://github.com/user-attachments/assets/a9776b23-9696-43e1-9f79-7a39e2e7f50d)

# CONCLUSIONS:
<b>How feature, 2ND PTSL3MA for Atlanta Hawks (ATL) compares to rest of league </b> <br>
<br>
![2ND PTSL3MA](https://github.com/user-attachments/assets/40c43748-1196-409b-b79e-bd3b7752fe12)

# CONCLUSIONS:
<b> How feature, OPP PTS OFF TOL1MA for Charlotte Hornets (CHA) compares to rest of league </b> <br>
<br>
![OPP PTS OFF TOL1MA](https://github.com/user-attachments/assets/ec0507c4-363b-45fb-a0cf-93b7cd8cecbd)

# CONCLUSIONS:
<b> How feature, PTS OFF TOL1MA for Los Angeles Clippers (LAC) compares to rest of league </b> <br>
<br>
![PTS OFF TOL1MA](https://github.com/user-attachments/assets/6c557ba9-6908-4f36-bd32-87483d410a20)
<br>
# CONCLUSIONS:
<b> How feature, FBPSL1MA for Oklahoma City Thunder (OKC) & Memphis Grizzlies (MEM) compares to rest of league </b> <br>
<br>
![FBPSL1MA](https://github.com/user-attachments/assets/7b9eefcf-8c95-4c94-9895-9a413e435e7b)


# PROFF 
![ORL_byOddsRatioTrue](https://github.com/user-attachments/assets/8b72f3af-5b04-4d3f-b582-53c8bf788b6e)
<br><br>
![true](https://github.com/user-attachments/assets/bc543685-82ae-48b7-bf31-03d231d615a0)
<br><br>
![ORL_byOddsRatioStandardized](https://github.com/user-attachments/assets/baf03fdb-3824-45d0-a9c6-eeb54120a8a9)
<br><br>
![standardized](https://github.com/user-attachments/assets/ef93a1da-1e23-4d49-b6c3-b47598f38991)
<br><br>
![ORL_byLogLossTrue](https://github.com/user-attachments/assets/ec0f87e6-7a36-4437-99cb-91b64ee56b25)
<br><br>
![ORL_byLogLossStandardized](https://github.com/user-attachments/assets/127adab7-d1dc-42a7-b73a-aa0644536ef8)





