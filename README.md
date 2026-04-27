Project Title
- Tennis Ace

Introduction 
- "Game, Set, Match!" No three words are sweeter to hear as a tennis player than those, which indicate that a player has beaten their opponent. A league of professionals spends day and night, month after month practicing to be among the best in the world.

Dataset
- The data was provided by Codecademy, under Machine Learning I project, obtained from men's professional tennis league, Association of Tennis Professionals (ATP) from the top 1500 ranked players over the span of 2009 to 2017.
- The dataset contains Player, Year, Aces, DoubleFaults, FirstServe, FirstServePointsWon, SecondServePointsWon, BreakPointsFaced, BreakPointsSaved, ServiceGamesPlayed, ServiceGamesWon, TotalServicePointsWon, FirstServePointsWon,FirstServeReturnPointsWon, SecondServeReturnPointsWon, BreakPointsOpportunities, BreakPointsConverted, ReturnGamesPlayed, ReturnGamesWon, ReturnPointsWon, TotalPointsWon, Wins, Losses, Winnings, and Rankings.

Objective
- Create a linear regression model that predicts the outcome for a tennis player based on their playing habits.

Methods
- Scatter plots are used to identify which features have a positive linear trend against the outcome 'Winnings', at a constant random_state of 66 to make sure results are consistent and reproducible.
- Once these feature are identified, linear regressions were done individually, by pair, and on multiple features to find out the best features.

Key Findings
- There were six features that produces positive linear trend based on the scatter plots, which are:
  1. Aces
  2. BreakPointsFaced
  3. BreakPointsOpportunities
  4. DoubleFaults
  5. ReturnGamesPlayed
  6. ServiceGamesPlayed
- Individually, based on their R² values in test set, these were three best features in predicting 'Winnings':
  1. ServiceGamesPlayed
  2. ReturnGamesPlayed
  3. BreakPointsOpportunities
- By pairs, these were three best pairs in predicting 'Winnings':
  1. BreakPointsFaced and ServiceGamesPlayed
  2. BreakPointsFaced and ReturnGamesPlayed
  3. ReturnGamesPlayed and ServiceGamesPlayed
- A model that uses all six features was also made. However the R² value of the test set shows a value equal to the two-features model (BreakPointsFaced and ServiceGamesPlayed).
- This suggests that extra features do not improve prediction and may be unnecessary.
- Two-features model (BreakPointsFaced and ServiceGamesPlayed) is preferred for interpretability and avoid overfitting.
