---
title: Preliminary research
sidebar_position: 4
---

# Preliminary Research
During our pre-research phase, we did not find many sources, which was both a motivation and a demotivation in that our subject is not overdone, but we also did not have a lot of inspiration to work from.

## Automatic Wordfeud Playing Bot
One source we made effective use of, is the [report][report_MB&FE] of a bachelor thesis by Martin Berntsson and Fredric Ericsson at the Royal Institute of Technology KTH in Sweden. They built a bot which followed the strategy of picking the move which resulted in the highest score in the current turn, what we call 'greedy'. The pseudo-code for the algorithm in the report was implemented in our bot code, forming the base of all types of bots we have produced. ([Berntsson & Ericsson, 2010][report_MB&FE]).

## General strategy

A lot matters when it comes to strategy in Wordfeud. It takes not just extensive reading in a dictionary to get good, and "The players at the top level tend to have some mathematical ability", as mentioned by Mina Le, ranked a hundred and tenth among Scrabble players in the US. One of the deciding factors to one's ability to play Scrabble or Wordfeud is knowledge of statistics: knowing the chances of you and your opponent receiving certain tiles, thinking a few turns ahead and using that mathematical brain to analyse the board. As single time North-American Scrabble champion Will Anderson said, "it's less of a word-finding game, and more of a word-picking game".([Aronow, 2023][column_NYT_Scrabble])

The points discussed above also apply to our Wordfeud bot. It tries to keep "good letters" on its tilerow by looking at the letters which are still left in the tilebag. The bot also reviews the options which are created for the opponent by playing its own word, and tries to minimalise the points it gives away.



[report_MB&FE]: https://www.csc.kth.se/utbildning/kth/kurser/DD143X/dkand12/Group3Johan/report/berntsson_ericsson_report.pdf
[column_NYT_Scrabble]: https://www.nytimes.com/2023/08/03/crosswords/scrabble-strategy-math.html