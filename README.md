# NBARankings

Data cleaning, analysis and statistical significance tests conducted in Google Colab. The Jupyter Notebook is included with all calculations ran using Python. 

Research Questions

At the conclusion of each NBA season a committee votes on the players most deserving for end-of-year accolades. The MVP ladder shows, in order, players ranked based on number of 1st, 2nd and 3rd place votes. The cumulative total crowns that season's Most Valuable Player. The exact methodology behind this process is not available for the public, but for the purposes of this analysis the final rank is of most importance.

Nate Silver of FiveThirtyEight developed an industry leading, widely recognized rating system titled "RAPTOR", which has analyzed every season since player tracking data was first implemented in 2013-2014. I will be using this rating system to develop a ranking of each season's top players.

As a point of comparison, I will also develop a rank based on 'traditional' metrics used to measure player performance. These are independent from the RAPTOR system, but integrate similar statistics interchangeably. The main difference is the weight placed on the inputs that make up the rating scale.

Datasets

RAPTOR The first dataset used is taken from FiveThirtyEight’s GitHub repository NBA-RAPTOR. This dataset contains Nate Silver’s current metric for rating NBA Players. The features within the dataset include a RAPTOR rating for offense and defense within the scopes of BPM (box) and RPM (on/off). Also included is the RAPTOR WAR (wins above replacement) metric which takes everything into account and produces the player’s impact on total team wins.

NBA The NBA / Box data is imported from Basektball-Reference. This rating system is built from existing sources in Box Plus / Minus (BPM), Value Over Replacement Player (VORP) and Win Share (WS). BPM is derived from a player’s box (score), which contains traditional statistics such as rebounds, field goal percentage, points per game, etc. VORP is based on a team’s performance when a player is either on or off the court. This is denoted as positive or negative, with the numerical value showing how much better or worse the team performs in that specific area relative to said player being on or off the court. Win Share is the player's contribution to team wins or losses

Voting I will also be using the end-of-year voting results imported from Basketball-Reference. This dataset will contain the variables from both RAPTOR and NBA systems, but will only account for the selection of players found in the voting results.
