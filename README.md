# PREDICT RESULTS OF 2023-24 NBA REGULAR SEASON GAMES WITH LOGISTIC REGRESSION 
## BY OLUTOSIN FASHUSI
<b><i> EXCERPT FROM NBA GAMES PLAYED ON 2024-02-22: </b></i>
<br><br>
![2024-02-22MatchResults](https://github.com/user-attachments/assets/376ab6ea-146f-4ed8-b322-a9d84505ab42)
• DATE: Date game played (Predictions begin on games played post-2024 All Star Game which was played on 2024-02-18) <br>
• MATCH: Team abbreviation of away team @ team abbreviation of home team <br>
• GAMEID: Every NBA game has a unique GAMEID <br>
• MODEL PREDICTS: Team abbreviation that model predicts to win <br>
• ACTUAL WINNER: (Team abbreviation that actually won the game, ✅ if model vs actual winner model prediction correct ❌ if incorrect) <br>
• BETTING FAVORITE: (Team abbreviation of betting favorite, match spread, ✅ if model vs betting favorite model prediction correct ❌ if incorrect)
# MATCH TRAIN & TEST DETAILS AND DECISION BOUNDARIES
## MATCH ORL @ CLE, GAMEID: 22300792 TRAIN & TEST DETAILS
![ORL@CLE_RESULTS](https://github.com/user-attachments/assets/7d42cece-b062-4be5-b21a-1a7b939ccd4d)
![ORL@CLE_MatchTestDetails](https://github.com/user-attachments/assets/a033fb2e-b2d6-49e0-8861-8474797a31ae)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH ORL @ CLE, GAMEID: 22300792 DECISION BOUNDARIES
![ORL](https://github.com/user-attachments/assets/aff57972-8b5a-45a9-b4fe-52bffa78d6d5)
![CLE](https://github.com/user-attachments/assets/6a7cef13-c2d5-4e2c-b419-3a2f078f4211)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Fast Break Points in last game played (FBPSL1MA) as best feature for team, ORL (Orlando Magic) <br>
•	Model identifies Opponent Points in the Paint in last game played (OPP PITPL1MA) as best feature for team, CLE (Cleveland Cavaliers) 
<br><br>
## MATCH DET @ IND, GAMEID: 22300793 TRAIN & TEST DETAILS
![DET@IND_RESULTS](https://github.com/user-attachments/assets/39d9a570-da1d-4bc7-a6e1-da0cd6f1be57)
![DET@IND_MatchTestDetails](https://github.com/user-attachments/assets/ccf9aef0-e3e4-49b5-84d3-6789b9d63fda)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH DET @ IND, GAMEID: 22300793 DECISION BOUNDARIES
![DET](https://github.com/user-attachments/assets/ec0d837d-84c7-4160-bf25-29ba34b5eb28)
![IND](https://github.com/user-attachments/assets/f2a69a8d-b60e-417a-b994-48ad5f5691c3)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Points in the Paint in last 4 games played (OPP PITPL4MA) as best feature for team, DET (Detroit Pistons) <br>
•	Model identifies Points off Turnovers in last game played (PTS OFF TOL1MA) as best feature for team, IND (Indiana Pacers)
<br><br>
## MATCH NYK @ PHI, GAMEID: 22300794 TRAIN & TEST DETAILS
![NYK@PHI_RESULTS](https://github.com/user-attachments/assets/5d3782f7-3d6a-4c57-87ef-7e7d74a70786)
![NYK@PHI_MatchTestDetails](https://github.com/user-attachments/assets/d0c1d9ea-ab3e-4a85-849f-2d4c265ca714)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH NYK @ PHI, GAMEID: 22300794 DECISION BOUNDARIES
![NYK](https://github.com/user-attachments/assets/256e3ff2-4df0-4d87-9708-81038949bdea)
![PHI](https://github.com/user-attachments/assets/3d6a6c5d-c8b6-432b-b98c-14b8b1b4b3a5)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Points off Turnovers in last 2 games played (PTS OFF TOL2MA) as best feature for team, NYK (New York Knicks) <br>
•	Model identifies Opponent Points off Turnovers in last 5 games played (OPP PTS OFF TOL5MA) as best feature for team, PHI (Philadelphia 76ers)
<br><br>
## MATCH BKN @ TOR, GAMEID: 22300795 TRAIN & TEST DETAILS
![TOR@BKN_RESULTS](https://github.com/user-attachments/assets/0f9ffb72-4c90-4fc2-9cc8-f8d61eb55e72)
![TOR@BKN_MatchTestDetails](https://github.com/user-attachments/assets/ca093c74-9070-4bc9-8d19-2ed9b208c9d7)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH BKN @ TOR, GAMEID: 22300795 DECISION BOUNDARIES
![BKN](https://github.com/user-attachments/assets/f5a86c9b-cb95-465d-a07b-cf76d12c226a)
![TOR](https://github.com/user-attachments/assets/e01d3ce7-c268-440f-a25d-ea4d686f9407)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Opponent 2nd Chance Points in last 5 games played (OPP 2ND PTSL5MA) as best feature for team, BKN (Brooklyn Nets) <br>
•	Model identifies Opponent 2nd Chance Points in last 2 games played (OPP 2ND PTSL2MA) as best feature for team, TOR (Toronto Raptors)
<br><br>
## MATCH PHX @ DAL, GAMEID: 22300796 TRAIN & TEST DETAILS
![PHX@DAL_RESULTS](https://github.com/user-attachments/assets/951b1ece-77e6-4b67-9cde-ae72d6dc4745)
![PHX@DAL_MatchTestDetails](https://github.com/user-attachments/assets/f5db8492-fbd0-4a05-aad6-cf22c6839c1b)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH PHX @ DAL, GAMEID: 22300796 DECISION BOUNDARIES
![PHX](https://github.com/user-attachments/assets/6e076d8f-638d-41c8-916a-7cf04a9cde21)
![DAL](https://github.com/user-attachments/assets/f5f3abee-92a3-4991-9a38-cbd550da6b7c)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Opponent 2nd Chance Points in last 3 games played (OPP 2ND PTSL3MA) as best feature for team, PHX (Phoenix Suns) <br>
•	Model identifies Opponent 2nd Chance Points in last game played (OPP 2ND PTSL1MA) as best feature for team, DAL (Dallas Mavericks)
<br><br>
## MATCH BOS @ CHI, GAMEID: 22300797 TRAIN & TEST DETAILS
![BOS@CHI_RESULTS](https://github.com/user-attachments/assets/b82f60b0-b6a9-4f3a-82f9-2b946dbf5a06)
![BOS@CHI_MatchTestDetails](https://github.com/user-attachments/assets/947dcf49-1089-4ee1-b1e0-9f66496d342e)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH BOS @ CHI, GAMEID: 22300797 DECISION BOUNDARIES
![BOS](https://github.com/user-attachments/assets/63f971ac-9d02-42b1-9027-adfc0dcba238)
![CHI](https://github.com/user-attachments/assets/e6966a89-83be-42dc-ae4c-e93eec5164a5)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Opponent Fast Break Points in last 5 games played (OPP FBPSL5MA) as best feature for team, BOS (Boston Celtics) <br>
•	Model identifies Opponent Points off Turnovers in last game played (OPP PTS OFF TOL1MA) as best feature for team, CHI (Chicago Bulls)
<br><br>
## MATCH HOU @ NOP, GAMEID: 22300798 TRAIN & TEST DETAILS
![HOU@NOP_RESULTS](https://github.com/user-attachments/assets/9e26a9d7-1161-4274-9386-ebc93a9ca991)
![HOU@NOP_MatchTestDetails](https://github.com/user-attachments/assets/62c172ed-c7cc-493d-ba93-334585d85987)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH HOU @ NOP, GAMEID: 22300798 DECISION BOUNDARIES
![HOU](https://github.com/user-attachments/assets/b69a4100-be18-4762-bc43-6b63404be897)
![NOP](https://github.com/user-attachments/assets/410051dc-66c3-4404-80a3-9c30840cd2bc)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Opponent Points off Turnovers in last 4 games played (OPP PTS OFF TOL4MA) as best feature for team, HOU (Houston Rockets) <br>
•	Model identifies Points off Turnovers in last game played (PTS OFF TOL1MA) as best feature for team, NOP (New Orleans Pelicans)
<br><br>
## MATCH LAC @ OKC, GAMEID: 22300799 TRAIN & TEST DETAILS
![LAC@OKC_RESULTS](https://github.com/user-attachments/assets/33345519-aab9-4cf1-895c-810bd6fa9113)
![LAC@OKC_MatchTestDetails](https://github.com/user-attachments/assets/40e5677b-8be2-4251-9e18-f09b37759aac)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH LAC @ OKC, GAMEID: 22300799 DECISION BOUNDARIES
![LAC](https://github.com/user-attachments/assets/0f6d1198-a43c-4e7f-8c1f-05ca21e9cfc9)
![OKC](https://github.com/user-attachments/assets/d2916eec-773f-4ea6-a6f2-10c963cd4f94)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Points off Turnovers in last game played (PTS OFF TOL1MA) as best feature for team, LAC (Los Angeles Clippers) <br>
•	Model identifies Fast Break Points in last game played (FBPSL1MA) as best feature for team, OKC (Oklahoma City Thunder)
<br><br>
## MATCH WAS @ DEN, GAMEID: 22300800 TRAIN & TEST DETAILS
![WAS@DEN_RESULTS](https://github.com/user-attachments/assets/48fcce5a-2dc4-47ee-914b-2f73810a1cd7)
![WAS@DEN_MatchTestDetails](https://github.com/user-attachments/assets/4b3c3d27-9274-4d69-bcd4-9a4fe655391f)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH WAS @ DEN, GAMEID: 22300800 DECISION BOUNDARIES
![WAS](https://github.com/user-attachments/assets/7a14e75f-4837-4edf-9aca-ccee9df72171)
![DEN](https://github.com/user-attachments/assets/4fe1ef7a-f101-4b68-afb0-bf504b4b9cb0)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Opponent Fast Break Points in last 3 games played (OPP FBPSL3MA) as best feature for team, WAS (Washington Wizards) <br>
•	Model identifies Second Chance Points in last game played (2ND PTSL1MA) as best feature for team, DEN (Denver Nuggets)
<br><br>
## MATCH CHA @ UTA, GAMEID: 22300801 TRAIN & TEST DETAILS
![CHA@UTA_RESULTS](https://github.com/user-attachments/assets/68cfe707-18d2-44e5-911f-42e02f92268f)
![CHA@UTA_MatchTestDetails](https://github.com/user-attachments/assets/d350fa43-3da9-4d47-bef7-baff212ad0cd)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH CHA @ UTA, GAMEID: 22300801 DECISION BOUNDARIES
![CHA](https://github.com/user-attachments/assets/94649217-925c-4136-9ed6-d56708a7680d)
![UTA](https://github.com/user-attachments/assets/856f87f6-b76f-4751-9f75-d9019b19e61b)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Opponent Points off Turnovers in last game played (OPP PTS OFF TOL1MA) as best feature for team, CHA (Charlotte Hornets) <br>
•	Model identifies Points off Turnovers in last 5 games played (PTS OFF TOL5MA) as best feature for team, UTA (Utah Jazz)
<br><br>
## MATCH LAL @ GSW, GAMEID: 22300802 TRAIN & TEST DETAILS
![LAL@GSW_RESULTS](https://github.com/user-attachments/assets/16f138a3-9705-4bd5-910e-db05d5f0eecd)
![LAC@GSW_MatchTestDetails](https://github.com/user-attachments/assets/a77ed801-67f9-4374-a232-f478058b2e55)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH LAL @ GSW, GAMEID: 22300802 DECISION BOUNDARIES
![LAL](https://github.com/user-attachments/assets/5b12029e-e251-43e6-ac70-f0e0019c4e17)
![GSW](https://github.com/user-attachments/assets/3c6689ac-7ffb-4f65-bdba-c32136cca6dd)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Opponent Fast Break Points in last game played (OPP FBPSL1MA) as best feature for team, LAL (Los Angeles Lakers) <br>
•	Model identifies Opponent 2nd Chance Points in last 2 games played (OPP 2ND PTSL2MA) as best feature for team, GSW (Golden State Warriors)
<br><br>
## MATCH SAS @ SAC, GAMEID: 22300803 TRAIN & TEST DETAILS
![SAS@SAC_RESULTS](https://github.com/user-attachments/assets/ec01087c-4a74-46d0-96f6-b35c95a87e23)
![SAS@SAC_MatchTestDetails](https://github.com/user-attachments/assets/6e563d55-dfce-409c-8b34-ca90f0fc215d)
• TRAIN SIZE: Number of applicable previous games used to train model <br>
•	FEATURE: Feature with largest odds ratio (also tested feature with lowest log loss) <br>
•	PREDICT X_test: X_test used in prediction <br>
•	T/S: Indicates if true/standardized value used in train <br>
• PROBABILITY ESTIMATE: Team with the larger probability estimate is predicted to be the winner
## MATCH SAS @ SAC, GAMEID: 22300803 DECISION BOUNDARIES
![SAS](https://github.com/user-attachments/assets/a3b37c11-3169-482b-8031-faa611ffd9ce)
![SAC](https://github.com/user-attachments/assets/070f6730-32cd-4b5e-ab9e-60f1e2abb3ca)
•	Created with mlxtend's [plot_decision_regions](https://rasbt.github.io/mlxtend/user_guide/plotting/plot_decision_regions/) <br>
•	White star is PREDICT X_test value location used for prediction <br>
•	In red region model predicts loss, in blue region model predicts win <br>
•	Black dots are results from previous games played at feature z-score <br>
•	Above & below black dots are actual results from previous games <br>
•	X Labels show feature information for team feature with largest odds ratio <br>
•	Model identifies Fast Break Points in last game played (FBPSL1MA) as best feature for team, SAS (San Antonio Spurs) <br>
•	Model identifies Opponent 2nd Chance Points in last game played (OPP 2ND PTSL1MA) as best feature for team, SAC (Sacramento Kings)
# OBJECTIVES:
•	For each of the 30 NBA teams, utilize data from previous games played to calculate probability estimate of team winning their next game <br>
•	Model predictions begin on games played post the NBA 2024 All Star Game played on 2024-02-18 <br>
•	Compare model's predicted winner to 1) actual winner 2) team listed as the betting favorite <br>
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
<b><i>VEGASINSIDER.com</i></b> <br>
&nbsp;&nbsp;&nbsp; [NBA Odds & Betting Lines](https://www.vegasinsider.com/nba/odds/las-vegas)
# CONCLUSIONS:
<b>PREDICTION RESULTS BY TEAM</b>
<br>
![percentCorrect](https://github.com/user-attachments/assets/f4bd464f-4f98-4a1a-99c6-d4528ec3c47e)
<b><i> Gaps exists because model makes 0 predictions of a Pistons win </i></b>
<br><br>
![numberCorrect](https://github.com/user-attachments/assets/d87384fe-95e5-4797-b5c8-fccc0a5adf93)
<b><i> Model correclty predicts a league high of 26 vs Actual Result & 21 vs Betting Favorite for Boston Celtics </i></b>
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
![sameFeatureATL](https://github.com/user-attachments/assets/8fe0d663-3432-439c-8022-28baab0b4350)
![2ND PTSL3MA](https://github.com/user-attachments/assets/40c43748-1196-409b-b79e-bd3b7752fe12)

# CONCLUSIONS:
<b> How feature, OPP PTS OFF TOL1MA for Charlotte Hornets (CHA) compares to rest of league </b> <br>
<br>
![sameFeatureCHA](https://github.com/user-attachments/assets/b800f251-e34f-46dd-95de-854489b56f00)
![OPP PTS OFF TOL1MA](https://github.com/user-attachments/assets/ec0507c4-363b-45fb-a0cf-93b7cd8cecbd)

# CONCLUSIONS:
<b> How feature, PTS OFF TOL1MA for Los Angeles Clippers (LAC) compares to rest of league </b> <br>
<br>
![sameFeatureLAC](https://github.com/user-attachments/assets/70e5d42d-651c-4897-b32a-78ec4493d487)
![PTS OFF TOL1MA](https://github.com/user-attachments/assets/6c557ba9-6908-4f36-bd32-87483d410a20)
<br>
# CONCLUSIONS:
<b> How feature, FBPSL1MA for Oklahoma City Thunder (OKC) & Memphis Grizzlies (MEM) compares to rest of league </b> <br>
![sameFeatureOKC_MEM](https://github.com/user-attachments/assets/6c609e90-a0a3-44e1-85c7-6a241a4d339a)
<br>
![FBPSL1MA](https://github.com/user-attachments/assets/7b9eefcf-8c95-4c94-9895-9a413e435e7b)


# PROFF: BY ODDS RATIO
![ORL_byOddsRatioTrue](https://github.com/user-attachments/assets/d7d43fbc-1e6e-4455-8efe-dd71d41f1a61)

![ORL_byOddsRatioStandardized](https://github.com/user-attachments/assets/2d13f34d-8581-42f3-92e2-c55a34838b16)

# PROFF: BY LOG LOSS
![ORL_byLogLossTrue](https://github.com/user-attachments/assets/91b8052e-0f9d-405a-bc9e-9bbc9608f2a0)

![ORL_byLogLossStandardized](https://github.com/user-attachments/assets/822612e8-3f12-44ff-8ac3-09bfcfb135ad)


# FURTHER QUESTIONS 
## TEAM WIN% AT HOME?
![recordAtHome](https://github.com/user-attachments/assets/d935e338-5e9e-4bc5-8a79-cc68fcdca53a)
## TEAM WIN% ON THE ROAD?
![recordRoad](https://github.com/user-attachments/assets/8feda766-cace-4a11-8d52-0e53915da681)
## TEAM  WIN% WITH 0 DAYS OFF?
![0DAYSOFF](https://github.com/user-attachments/assets/1690a4f8-1e0a-4fe8-8454-2c92f73229fb)
## TEAM  WIN% WITH 1 DAY OFF?
![1DAYOFF](https://github.com/user-attachments/assets/93392b93-510c-4f44-b9e0-761a9abb5afd)
## TEAM  WIN% WITH 2 DAYS OFF?
![2DAYSOFF](https://github.com/user-attachments/assets/a5689a5c-57c5-44a0-8414-c2f337a621bb)
## TEAM  WIN% WITH >2 DAYS OFF?
![moreThan2DAYSOFF](https://github.com/user-attachments/assets/91c1b630-037e-4bab-8849-a3cc88193963)
