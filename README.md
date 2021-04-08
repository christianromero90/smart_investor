# Fintech

This is a project from the course ***Fintech*** which is a part of **Hult's MSc. in Finance program in Boston**.

## goal:
Develop Robo-Advisor as explained in the links on Canvas. You do not need to have all parts working perfectly. I suggest first completing the analytics part in python code directly rather than worrying too much about interactive or web-based plots. Do the analysis first and add in the interactive parts/graphs later. 

## Smart investor:
### risk assesment
Smart investor is a simple investment advisor that takes into consideration users risk aversion by scoring answers of an initial questionnaire. The results of this assesment can be 5 different types of profiles ranging from conservative to aggresive with its respective capital allocation.

### previous holdings
Smart investor will also ask users for any stocks that they already own, how many do they possess and when did they acquire them. It will perform an initial optimization maximizing sharpe ratio and finding the optimal weights. The lookback period is fixed but it can be set so users can specify it. The lookback period used to calculate expected returns of stocks and their volatility is from 2015-01-01 until yesterday (to ensure available closing prices).

A graphical representation of the MU-SIGMA with the maximum Sharpe portfolio is displayes, as well as a pie chart with the optimized weights.

So even if a user is not adding new stocks to his/her portfolio, this initial section will suggest the best weights to have in his/her user's current holdings.

## add stocks
If there are any stocks that the user is interested in owning, Smart-Investor will obtain the neccesary data and using Modern Portfolio Theory will determine if these should be added to the portfolio or not using the prtfolio improvement rule:

[Portfolio improvement](Port_improv_rule.png)

## Monte Carlo Simulation
Using Monte Carlo to simulate cummulative returns using the optimized portfolio mean and standard deviation drawn from a normal distribution.
