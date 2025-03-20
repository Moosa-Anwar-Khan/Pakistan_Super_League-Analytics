I worked on project in which I was provided with data of PSL players. My task was to select 16 men squad for  T20 team of Pakistan. I was provided with
unlabeled data so I decided to perform unsupervised learning (K-means clustering) on both batsmen and bowlers. Following are the steps which will 
help you to understand what I have done. 


1) First I performed clustering on "batsmen.csv" (clustering was performed on the basis of batsman's "innings", "strike rate" and "average") and "bowlers.csv" 
(clustering was performed on the basis of  bowler's "economy", "strike rate" and "average").

2) After performing clustering I created "batsmenLabel.csv" and "bowlersLabel.csv"

3) Then I performed analysis for batsmen and bowlers which can be found in jupyter file named, "analysisForBatsmen" and "analysisForBowlers".

4) After performing analysis for bowlers and batsmen, I created csv file for selected batsmen and bowlers namely, "batsmenSelected.csv" and "bowlersSelected.csv". 
I selected 9 batsmen and 7 bowlers for team.

5) I also performed decision tree classification which is supervised learning technique on files, "batsmenLabel.csv" and "bowlersLabel.csv" so that I can predict 
the class of player by entering his "strike rate", "average" and "innings" incase of bastmen and "strike rate", "average" and "econony" incase of bowlers.  