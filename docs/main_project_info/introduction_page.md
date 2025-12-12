---
title: Project Introduction
sidebar_position: 1
---

# Introduction to our PWS

Welcome again! Seeing as you have chosen to read through the *Main Project* documentation, we assume that you are either interested in us due to the fact that this is a PWS, or you are just interested in the development process in general. We hope to provide you with enough information about everything related to the project. 

## Motivations behind the project

We are Stijn and Joram. As we mentioned before, this project is our PWS. We had the immense luck that we went through secondary education at a school which provided Computer Science as an option for our courses, and we have both enjoyed the subject to such an extent that the decision to do our PWS in it was quite easy.  
Our supervisor, [Marten Postma][PostmaGithub], has helped us along the way to take a step back and evaluate. He also gave us the idea to, instead of creating a standard text document for our report, launch this website to broaden our audience and give people a better understanding of what our bot is and how it came to be.  
We chose to create our WordFeud bot using the programming language Python, as it the language we are both most experienced and proficient with.

## Goals

The main goal for our project was to create a bot for the digital game WordFeud which makes its decisions based entirely on hardcoded instructions. This means that we have steered clear from AI and Machine Learning so that our product follows steps of reasoning we can trace directly and to great detail. We decided to go for this path because we wanted to see how advanced we could make such a bot in the period of time we had while maintaining a level of enjoyment we could have playing the original game. From this core idea, we constructed a few sub-goals.
1. Define a WordFeud strategy based on our own experience and that of professional WordFeud players we can reach.
2. Transform this WordFeud strategy into basic logic.
3. Design 3 bots that play based on different components of said strategy.
    1. Design a bot which chooses the move which, in the current turn, results in the greatest increase in score.
    2. Design a bot which takes both the current increase in score and the chance it will be able to play all 7 letters in the next turn into account to choose the best move.
    3. Design a bot which takes both the current increase in score and the situations which that move create on the board into account to choose the best move.
4. Design a 4th bot which combines the components of the last two mentioned bots to come to a strategy which reflects the originally drafted tactic.
5. Analyse scores and playing speed in a multitude of matchups between the different types of bots to see which is the strongest while remaining an opponent a human can also play against.

We want to elaborate a bit further on these subgoals to make them even clearer without creating multi-sentence stories for each of them.  
Subgoal 2 means that we attempt to reshape our chosen strategy to be more concise and then form a ruleset from it to dictate what the bot is supposed to base its decisions on.  
Subgoal 3.1 outlines the bot which we call Greedy, subgoal 3.2 shows the Chance bot and subgoal 3.3 is about the Boardposition bot. Subgoal 4 describes the Combi bot. The mechanisms which ultimately drive these 4 bots are described in the *Bot Information* section of the *Main Project* path.
Subgoal 5 mentions the bot remaining a playable opponent. This means that it can play on its own and that it chooses its moves in a time of **... (add time)** which we find acceptable.


[PostmaGithub]: https://github.com/MartenPostma