---
title: Conclusions
sidebar_position: 6
---

# Conclusions

From the three matchups between the bots that we simulated, we have been able to form the following conclusions and results for our main- and sub-goals, which we will repeat below.
* Create a bot that can play based on a complete strategy we formulated while maintaining a reasonable time per move of 90 seconds.
1. Define a Wordfeud strategy based on our own experience and that of professional Wordfeud players we can reach.
2. Transform this Wordfeud strategy into basic logic.
3. Design three bots that play based on different components of said strategy.
    1. Design a bot which chooses the move which, in the current turn, results in the greatest increase in score.
    2. Design a bot which takes both the current increase in score and the chance it will be able to play all seven letters in the next turn into account to choose the best move.
    3. Design a bot which takes both the current increase in score and the situations which that move create on the board into account to choose the best move.
4. Design a fourth bot which combines the components of the last two mentioned bots to come to a strategy which reflects the originally drafted tactic.
5. Analyse scores and playing speed in a multitude of matchups between our different bots to see which is the strongest while remaining an opponent a human can also play against.

For subgoal 1 and 2, we can conclude that the strategy the bot ultimately follows is a partial version of the strategy we originally created due to limitations computing power put on the number of calculations it could do in the move time mentioned in the main goal.

For subgoal 3.1, the Greedy bot is the result. When analysing the moves it made in the matchups, we conclude that this part has ended in success as we cannot find moves that give a higher number of points.  
For subgoal 3.2, the Chance bot is the product. Here, the hypothesis also turns out correct. In the matchup between Chance and Greedy, Chance wins more often than Greedy and it correctly calculates chances.
For subgoal 3.3, the Boardposition bot is the product. The sub-hypothesis for this goal is found incorrect, as Boardposition loses more often than it wins from Greedy, although it does base its decision on the strategy mentioned.
From these three sub-goals, a conclusion is formed that the hypothesis 3 is incorrect, as only two out of three sub-hypotheses are correct.  

Subgoal 4 has been finished with success, and the hypothesis is also found correct. the Combi bot, which is the result of this goal, makes decisions which we find logical based on our own strategy.

Subgoal 5 has also been completed successfully, as Combi wins more often than it loses from Greedy and it maintains a move time below 90 seconds.

Thus, we can conclude that the main goal is successful since the Combi bot achieves all benchmarks set for it, even though not all sub-goals are accomplished.