---
title: Research
sidebar_position: 5
---

# Research

As mentioned in Methodology, our design process included long and thorough simulation. From those simulation logs, we were able to do some research. The main results of that research are summarized in the table provided below.

| Bot 1 | Bot 2 | Wins bot 1 | Wins bot 2 | Win % bot 1 | Win % bot 2 | Avg. score bot 1 | Avg. score bot 2 | σ bot 1 | σ bot 2 | t̅ bot 1 | t̅ bot 2 |  
| - | - | - | - | - | - | - | - | - | - | - | - |
| Greedy | Chance | 26 | 35 | 42.6% | 57.4% | 479 | 493 | 49.9 | 65.6 | 18.85 | 42.89 |  
| Greedy  | Boardposition | 51 | 34 | 60% | 40% | 448 | 433 | 57.6 | 60.4 | 19.34 | 21.18 |  
| Greedy  | Combi | 45 | 57 | 44.1% | 55.9% | 464 | 500 | 65,2 | 69,9 | 22.50 | 44.21 |  

Clarification for the table:
* Avg. score: the average score the bot had after the game ended.
* σ: the standard deviation from the average score.
* t̅: the average time taken per move in seconds.
* Win %: percentage of wins compared to the total number of matchups.

## Observations from the results

There are a few notable observations to be made when reviewing these statistics.  
Firstly, an incredibly interesting set of numbers are the win percentages. Although the Combi bot was supposed to be the strongest bot and should have thus had the lowest win percentage, Chance actually has a better one. Meanwhile, Boardposition has, as the only one of the 'more advanced' bots, a win percentage below 50%.
Firstly, it is interesting to see that in the matchup between Greedy and Boardposition, the win-lose ratio for Greedy is 51-34. This means that Boardposition is the only 'more advanced' bot that has lost to Greedy more often than it has won. This observation does have more context to be placed in, that being the average score. Comparing the average score of Greedy between its matchup against Chance and its games with Boardposition shows a decrease in the average score of more than thirty points. These lower scores might be due to the mostly defensive strategy of Boardposition, which prevents Greedy from getting high scoring moves. Accordingly, to our hypothesis, Combi has the highest average score of any bot, although Greedy also has a higher average in that matchup.

Secondly, the average time per game is a statistic where a major difference is to be spotted. Chance takes more than twice as long as Greedy in its own matchup, and there is also a comparable factor between its time and the times in the Greedy vs. Boardposition matches. Combi takes after Chance when looking at these times, with an average only 9 seconds lower than that of Chance.