I worked on a project in which I was provided with data on PSL players. My task was to select a 16-man squad for the T20 team of Pakistan. I was provided withunlabeled data, so I decided to perform unsupervised learning (K-means clustering) on both batsmen and bowlers.

Following are the steps that will Help you to understand what I have done.

1) First I performed clustering on "batsmen.csv" (clustering was performed on the basis of the batsman's "innings", "strike rate" and "average") and "bowlers.csv" (clustering was performed on the basis of the bowler's "economy", "strike rate" and "average").

For Batsman:
   - **Innings**: A period of batting in a match where a batsman faces deliveries.
   - **Strike Rate**: The number of runs a batsman scores per 100 balls faced.
   - **Average**: The average number of runs a batsman scores per dismissal (total runs divided by the number of times out).

For Bowlers:  
   - **Economy**: The number of runs a bowler concedes per over bowled.
   - **Strike Rate**: The number of balls a bowler takes to dismiss a batsman.
   - **Average**: The average number of runs a bowler gives per wicket taken (total runs conceded divided by the number of wickets taken).

2) After performing clustering, I created "batsmenLabel.csv" and "bowlersLabel.csv". The labels for batsmen and bowlers were generated on the basis of clustering. The labels for batsmen are "average_performer",     "good_performer", and "power_hitter". The labels for bowlers are "expensive_bowler" (meaning the bowler has given a lot of runs/score to opponents while bowling), "good_bowler", and "key_bowler".


3) Then I performed analysis for batsmen and bowlers which can be found in the Jupyter files named "analysisForBatsmen.ipynb" and "analysisForBowlers.ipynb".


4) After performing analysis for bowlers and batsmen, I created csv file for selected batsmen and bowlers, namely, "batsmenSelected.csv" and "bowlersSelected.csv". I selected 9 batsmen and 7 bowlers for the team.


5) I also performed decision tree classification, which is a supervised learning technique, on the files "batsmenLabel.csv" and "bowlersLabel.csv" so that I can predict the class of player by entering his "strike rate", "average" and "innings" in case of batsmen, and "strike rate", "average" and "economy" in case of bowlers. 
