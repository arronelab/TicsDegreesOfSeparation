# TicsDegreesOfSeparation
A bit of fun trying to see if an inside joke has any data to back it up.

Whenever I watch a match with friends or family, it isn't long before my classic line of "Used to play for Wigan him" comes out. I decided I should actually try to look it up and see if all roads really do lead to Wigan pier. To do this I:
* Used BeautifulSoup to scrape all the teams to appear in England's top 5 leagues for the past 5 seasons and collect all the currently listed squad members for these teams.
* Extracted the career of each of these players, teams played for with dates to/from, using pandas DataFrames to store this.
* Used python's networkx module to build a graph with players and teams as vertices, and edges between a player and every team they played for, and between players that played for the same team at the same time.
* Used shortest path algorithms to find the distance between any player and Wigan.
* Used centrality to measures to discover that unfortunately Wigan is not the centre of the footballing universe... but Luke Thomas is?
