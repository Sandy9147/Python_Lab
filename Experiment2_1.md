#Aim
To write a Python program to evaluate a cricket player’s batting, bowling, and fielding performance using conditional statements.

#Algorithm
Step 1: Start the program.
Step 2: Input the number of runs scored by the player.
Step 3: Input the number of balls faced.
Step 4: Input the number of wickets taken.
Step 5: Input the number of overs bowled.
Step 6: Input the number of runs conceded.
Step 7: Input the number of catches taken.
Step 8: Calculate Strike Rate (SR) using
SR = (Runs / Balls) × 100.
Step 9: Display the strike rate.
Step 10: Evaluate batting performance using conditions:
If runs ≥ 50 and SR ≥ 120 → Excellent Batter
If runs ≥ 30 and SR ≥ 100 → Good Batter
If runs ≥ 20 → Average Batter
Else → Poor Batter
Step 11: Calculate Economy Rate (ER)
ER = RunsConceded / Overs
Step 12: Display economy rate.
Step 13: Evaluate bowling performance:
If wickets ≥ 3 and ER ≤ 6 → Excellent Bowler
If wickets ≥ 2 and ER ≤ 8 → Good Bowler
If wickets ≥ 1 → Average Bowler
Else → Poor Bowler
Step 14: Evaluate fielding performance:
If catches ≥ 2 → Outstanding Fielder
If catches = 1 → Active Fielder
Else → Needs Improvement
Step 15: Stop the program.

#Python Code

runs = int(input("Enter the runs: "))
balls = int(input("Enter the number of balls: "))
wicket = int(input("Enter the number of wickets: "))
overs = int(input("Enter the number of overs: "))
runsconceded = int(input("Enter the runs conceded: "))
catches = int(input("Enter the number of catches: "))
# Strike Rate
SR = (runs/balls)*100
print(SR)
# Batter performance
if runs >= 50 and SR >= 120:
    batter = "Excellent Batter"
elif runs >= 30 and SR >= 100:
    batter = "Good Batter"
elif runs >= 20:
    batter = "Average Batter"
else:
    batter = "Poor Batter"
print(batter)
# Economy Rate
ER = runsconceded / overs
print(ER)
# Bowler performance
if wicket >= 3 and ER <= 6:
    bowler = "Excellent Bowler"
elif wicket >= 2 and ER <= 8:
    bowler = "Good Bowler"
elif wicket >= 1:
    bowler = "Average Bowler"
else:
    bowler = "Poor Bowler"
print(bowler)
# Fielder performance
if catches >= 2:
    print("Outstanding Fielder")
elif catches == 1:
    print("Active Fielder")
else:
    print("Needs Improvement")
    
Output
Enter the runs: 148
Enter the number of balls: 48
Enter the number of wickets: 5
Enter the number of overs: 2
Enter the runs conceded: 45
Enter the number of catches: 3
308.33
Excellent Batter
22.5
Average Bowler
Outstanding Fielder
Needs Improvement
