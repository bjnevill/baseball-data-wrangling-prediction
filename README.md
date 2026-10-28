# Baseball Data Wrangling & Next-Season Home Run Prediction

**Individual academic project · Ngee Ann Polytechnic, Diploma in Data Science · 2026**

Prepared a player–season dataset from multiple historical baseball tables to estimate a player's **home runs in the next recorded season**.

## Business-style question
Can current batting statistics, age, batting hand and All-Star selection help predict next-season home runs?

## Data wrangling
- Combined **batting**, **player** and **All-Star** records with carefully chosen join keys.
- Aggregated repeated player-year records before joins to avoid multiplying rows across team stints.
- Created a next-season target using a shifted helper table, while keeping the original season features unchanged.
- Limited scope to returning players from **1933–2014**; treated absent future outcomes as unknown rather than imputing the target.
- Applied numerical median and categorical mode imputation fitted on training data only.
- Investigated outliers, percentile capping and Yeo–Johnson transformations rather than assuming more processing always improves a model.
- Evaluated regression predictions against a naïve baseline.

## Tools
Python · pandas · NumPy · Data Joins · Data Cleaning · Time-Aligned Targets · Feature Engineering · scikit-learn

## Source files
The cleaned notebook package has been prepared separately. **The notebook has not yet been pushed to this repository.** Original course datasets are not redistributed.

*Educational analysis based on historical MLB data.*
