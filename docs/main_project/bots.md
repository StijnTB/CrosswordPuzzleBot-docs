---
title: Bot Information
sidebar_position: 4
---


# Bot strategies

The four bots we made - Greedy, Chance, Boardposition and Combi - all have (partially) different strategies which influence their playing style and results in matchups. Here, we will attempt to describe these strategies without going too deep into the complication of the actual code.

## Greedy

The Greedy bot makes its decisions based on one simple question: what move immediately gives me the highest number of points? This principle forms the base of the other three bots.
Greedy cannot to swap letters, so when it has no moves remaining it will always pass. The code used for this bot was, as mentioned earlier, taken from the [bachelor thesis][report_MB&FE] by Berntsson and Ericsson.

## Chance

The Chance bot adds to the Greedy principle with its *bingo_bonus_score*: a score between 0 and 100 which shows the chance it will be able to play a bingo in the next move. The higher this score, the better the move is.
The bot first calculates the chance to, in the next turn, have the letters to make a bingo for every possible letter combination that could remain on its tilerow. This chance is based on the letters in its own tilerow, and the letters remaining in the tilebag and on the opponents tilerow. The opponents tilerow is used in this calculation because the bot technically does not know what letters they have. To prevent a move taking hours due to extreme amounts of calculations necessary, we cap the options off at four hundred thousand. After the move has received a *bingo_bonus_score*, a total score is used to compare the current move with the best move. this total score is the base score of the word + the bingo chance * *reduction_multiplier*. Here, the multiplier is a float between zero and one. 
The Chance bot also allows for swapping letters, if the *bingo_bonus_score* for swapping those letters is high enough.

## Boardposition

The Boardposition bot has the most strategic potential between itself and the Chance bot. it calculates a *boardposition_score* based on dangerous situations a move creates. this score is then subtracted from the base score to calculate the total score used for comparing moves.
The first part of the *boardposition_score* is the expected multiplication. For every tile played in a move, an expected multiplication is calculated which is a factor the bot expects to see a new word played over that tile to get due to bonus tiles. the influence those tiles have on the expected multiplication decreases the further they are from the played tile.
The second part are prefixes and suffixes. Every word in the main word list also has an entry in the prefix- and suffix lists if there can be letters added before or after it. More possible additions result in a higher *boardposition_score*.
The third part is the danger of a word being played alongside the main word. This is limited to words ending next to the first tile, and words starting next to the last tile.
The Boardposition bot does not handle swapping letters, because the score of all possible letter swaps would be the same.

## Combi

The Combi bot, as its name suggests, combines both the Chance and Boardposition bot components to double the strategic potential. The combination of their strategies has resulted in a playstyle which fits with what we originally drafted up. For this bot, the comparison scores are calculated by adding the *bingo_bonus_score* to and subtracting the *boardposition_score* from the base score, after multiplying them by a factor between zero and one to let the performance adhere to our ideas of a good move.


[report_MB&FE]: https://www.csc.kth.se/utbildning/kth/kurser/DD143X/dkand12/Group3Johan/report/berntsson_ericsson_report.pdf