# beyond-the-scoreboard-scientific-visualization
This Scientific Visualization project reflects on how to analyse a football match based on the data, emphasizing on whether or not the domination on the field is reflected by the result on the scoreboard. For this project we have used the open data set published MD Mominul Islam (see CITATION.cff)

## Data
Data was retrieved from the [The FIFA World Cup 2026 Master Dataset](https://zenodo.org/records/21592427), containing **data for the 48 teams and the 104 matches** occurred during the **FIFA World Cup 2026**, hosted for the first time by three nations: USA, Canada and Mexico.

The dataset contained also **bio-metric information about the players** who took part in the competition, **venue-elevation data** and metrics such as **xG** (expected goals).

## Two hypothesis
1- Do xGs, ball possession and shots describe the result?
2- Are there any unexpected results?

## Results
1- From our analysis, made with k-means on k = 4, it occurred that **teams who were more forward-oriented and dominating** presented an **higher xG than the opponents**, leading to a victory in more than 80% of matches. Our clusterization also highlighted a difference between best and worst teams in an equilibrated match, with the **better equilibrated team** achieving 55% of wins, presenting only a **xG only 0.5 higher** than the opponents.
2 - After creating a **performance index** for each team, we clusterized using k-means for k = 2, and also implementing the **goal index**. We found that **14 matches** out of the 104 taken in exam were marked as **unexpected**: the performance index provided us also a list of the 10 most unexpected games, based on the difference in performance between the two teams playing.

## Limitations & future works
- Data about the **center of gravity** for each team could be an interesting metric to understand how much a team is pushing.
- **Temporal statistics** describing the evolution of the metrics used (e.g. ball possession throughout the match) could underline how and when a team is looking for the goal.
- **Predictive models** could be trained on this dataset, creating a generalized model that could work on any kind of football match.
- **Further analysis on team composition**, such as adding to the analysis the players actively in the match and how they change the team balance.

---

# How to Run it

## Folder Contents