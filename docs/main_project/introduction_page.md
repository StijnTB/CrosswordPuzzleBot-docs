---
title: Project Introduction
sidebar_position: 1
---

# Introduction to our PWS

Welcome again! Since you have chosen to read the *Main Project* documentation, we assume that you are either interested in us because that this is a PWS, or you are just interested in the development process in general. We hope to provide you with enough information about everything related to the project. 

## Motivations behind the project

We are Stijn and Joram. As we mentioned before, this project is our PWS. We were lucky to go through secondary education at a school that provided Computer Science as an option for our courses, and we have both enjoyed the subject to such an extent that the decision to do our PWS in it was quite easy.  
Our supervisor, [Marten Postma][PostmaGithub], has helped us along the way to take a step back and evaluate. He also gave us the idea to, instead of creating a standard text document for our report, launch this website to broaden our audience and give people a better understanding of what our bot is and how it came to be.  
We chose to create our Wordfeud bot using the programming language Python, as it the language we are both most experienced and proficient with.

## Goals

The main goal for our project was to create a bot for the digital game Wordfeud which makes its decisions based entirely on hardcoded instructions. This means that we have steered clear from AI and Machine Learning so that our product follows steps of reasoning we can trace directly and to detail. We decided to go for this path because we wanted to see how advanced we could make such a bot in the period we had while maintaining a level of playability we had while playing original game, with a reasonable reaction time from the bot. From this core idea, we constructed seven sub-goals.
1. Define a Wordfeud strategy based on our own experience and that of professional Wordfeud players we can reach.
2. Transform this Wordfeud strategy into basic logic.
3. Design three bots that play based on different components of said strategy.
    1. Design a bot which chooses the move which, in the current turn, results in the greatest increase in score.
    2. Design a bot which takes both the current increase in score and the chance it will be able to play all seven letters in the next turn into account to choose the best move.
    3. Design a bot which takes both the current increase in score and the situations which that move create on the board into account to choose the best move.
4. Design a fourth bot which combines the components of the last two mentioned bots to come to a strategy which reflects the originally drafted tactic.
5. Analyse scores and playing speed in a multitude of matchups between our different bots to see which is the strongest while remaining an opponent a human can also play against.

We want to elaborate a bit further on these subgoals to make them even clearer without creating multi-sentence stories for each of them.  
Subgoal 2 means that we attempt to reshape our chosen strategy to be more concise and then form a ruleset from it to dictate what the bot is supposed to base its decisions on.  
Subgoal 3.1 outlines the bot which we call Greedy, subgoal 3.2 shows the Chance bot and subgoal 3.3 is about the Boardposition bot. Subgoal 4 describes the Combi bot. The mechanisms which drive these four bots are described in the *Bot Information* section of the *Main Project* path.
Subgoal 5 mentions the bot remaining a playable opponent. This means that it can play on its own and that it chooses its moves in a time of around 90 seconds which we find acceptable.

## Hypotheses

We have formed the following hypothesis for our main goal: the bot plays Wordfeud on a level that allows it to make a move that follows our strategic plan in under 90 seconds.  
Supporting this are our sub-hypotheses, ordered in the same way as the sub-goals:
1. The strategy followed by the bot (partially) matches the strategy we laid down based on our research.
2. The code for the bot follows the strategy mentioned in sub-hypothesis one.
3. The bots' playing strength and playing speed vary based on its components.
    1. The bot chooses the move that gives it the highest number of points.
    2. The bot beats the bot described in sub-goal 3.1 and bases its decision for the move on both the number of points the move gives and the chance it will be able to play a bingo in the next turn.
    3. The bot beats the bot described in sub-goal 3.1 and bases its decision for the move on both the number of points the move gives and the dangerous situations the move creates which the opponent might exploit.
4. The bot successfully combines the components mentioned in sub-goals 3.2 and 3.3 into a strategy that results in moves we find logical following our own knowledge of the game and strategy.
5. The bot achieves scores higher than those of the individual components mentioned in sub-goals 3.1 to 3.3 and maintains a playing speed below 90 seconds per move.



[PostmaGithub]: https://github.com/MartenPostma