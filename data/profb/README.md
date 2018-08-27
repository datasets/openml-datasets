The resources for this dataset can be found at https://www.openml.org/d/470

Author: Hal Stern, Robin Lock  
Source: [StatLib](http://lib.stat.cmu.edu/datasets/profb)   
Please cite:   

PRO FOOTBALL SCORES  (raw data appears after the description below)

How well do the oddsmakers of Las Vegas predict the outcome of
professional football games?  Is there really a home field advantage - if
so how large is it?  Are teams that play the Monday Night game at a
disadvantage when they play again the following Sunday?  Do teams benefit
from having a "bye" week off in the current schedule?  These questions and
a host of others can be investigated using this data set.

Hal Stern from the Statistics Department at Harvard University has
made available his compilation of scores for all National Football League
games from the 1989, 1990, and 1991 seasons.  Dr. Stern used these data as
part of his presentation "Who's Number One?" in the special "Best of
Boston" session at the 1992 Joint Statistics Meetings.

Several variables in the data are keyed to the oddsmakers "point
spread" for each game.  The point spread is a value assigned before each
game to serve as a handicap for whichever is perceived to be the better
team.  Thus, to win against the point spread, the "favorite" team must beat
the "underdog" team by more points than the spread.  The underdog "wins"
against the spread if it wins the game outright or manages to lose by fewer
points than the spread.  In theory, the point spread should represent the
"expert" prediction as to the game's outcome.  In practice, it more usually
denotes a point at which an equal amount of money will be wagered both for
and against the favored team.

Raw data below contains 672 cases (all 224 regular season games in
each season and informatino on the following 9 varialbes:     .

Home/Away       = Favored team is at home (1) or away (0)
Favorite Points = Points scored by the favored team
Underdog Points = Points scored by the underdog team
Pointspread     = Oddsmaker's points to handicap the favored team
Favorite Name   = Code for favored team's name
Underdog name   = Code for underdog's name
Year            = 89, 90, or 91
Week            = 1, 2, ... 17
Special         = Mon.night (M), Sat. (S), Thur. (H), Sun. night (N)
ot - denotes an overtime game