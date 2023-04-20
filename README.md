# Reinforcement-Learning-For-Portfolio-Management

![download (4)](https://user-images.githubusercontent.com/103140702/233470094-62b07402-cd74-48af-a07f-aff9b1633db5.png)


In this project, I experiment with constructing a reinforcement learning environment to teach a network how to balance an actively managed portfolio.  I create a portfolio of six commonly-traded large-cap stocks and manipulate this data to provide common financial metrics such as volatility, log return, expected returns, and asset betas.  Data is sourced from Bloomberg and backtestmarket.com.

I then calculate portfolio weights across the entire timespace using three different techniques, the Sharpe Ratio, the minimum variance technique, and the maximum diversification technique.  I chose to use the Sharpe and maximum diversification techniques as the two possible actions for the network, as one is high-risk and one is lower-risk.

After running three models, PPO, A2C, and TRPO, consistent outperformance of an evenly-weighted portfolio is achieved across all models.  The metric of greater interest is outperformance of the individual portfolio strategies (the Sharpe Ratio and maximum diversification).  Not all iterations of the models demonstrate this, but TRPO and PPO achieve this most consistently.

Further steps are to improve reproducibility of portfolio strategy outperformance and to test in more diverse environments.

Data is included in the Data folder.  The code is included as Reinforcement-Learning-Final.  The associated presentation is included as Presentation-Slides.
