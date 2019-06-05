---
layout: post
title: Examples
permalink: /examples.html
---

# Master's Thesis

Regulating the stock market is a tremendous undertaking, and it is vital to its safety and success. Many new regulatory issues have arisen along with the prevalence of electronic trading. One of these issues is known as maker-taker fees, which are essentially a means for stock exchanges to incentivize traders to offer liquidity at their venue. These fees were initially regulated at the beginning of the rise of electronic trading, but many argue this regulation needs to be updated to keep up with the practices that have evolved regarding the use of the fees. My thesis describes an agent-based model with minimally intelligent traders interacting in an artificial stock market with maker-taker fees. The purpose is to shed light on the effects of maker-taker fees as well as provide insight into the usefulness of agent-based modeling as a supplemental tool for regulatory decision-making. Results from the study show that maker-taker fees positively affect traditional measurements of market quality, and that minimal intelligence is a viable assumption for traders when modelling the stock market as long as a realistic market structure is present. This research aims to be a step toward incorporating agent-based models into exploratory groundwork for regulatory decision-makers at the Securities and Exchange Commission and other financial market regulatory agencies.  

The first chart below simply shows how the prices at two different exchanges in the model are generally entangled, but can depart from each other. The desire of the traders to receive the best price prevents an unlimited divergence, but the complex entrance of order placement and cancellations allows for global volatility as well as inter-exchange discrepancies.  

The second chart shows that the model produces a realistic price history through the trading activity of the agents. The zoomed area on the left side of the figure is roughly 1/10 of the total price history, while the zoomed area on the right side is roughly 1/100. There is a general resemblance in the pattern at each time scale. This is indicative of fractal patterns, which are not ambiguous since empirical price histories also show this fractal structure. In fact you can measure and compare two time series' [fractal dimensions](https://www.stat.washington.edu/sites/default/files/files/reports/2010/tr577.pdf). The fractal dimension of Microsoft's stock price history from 2014 to 2018 is 1.61, while the model produces a price history with a fractal dimension of 1.59 (very similar).

![Price Match](/images/PriceMatch.png) ![Fractal Price](/images/FractalPrice.png)  

The figure below demonstrates some of the results from my thesis. The time-weighted quoted spread is essentially a measure of the average difference between the best price a trader could get for selling and the best price for buying. This is known as the bid-ask spread, and smaller spreads are considered to indicate higher market quality. You can see that as the maker-taker fee increases, the average spread decreases, and therefore market quality is enhanced in the presence of the fees and their associated rebates. However, this is controversial since some argue that the market quality gains are artificial and therefore misleading to market participants and regulators. Agent based models have the potential to increase our understanding of the complex causal relationships between trading behavior, market structure, and regulation.

![Time Weighted Quoted Spread](/images/TWQS.png)

# Bank Reserves

This is an example of a very simple agent based model designed to explore the effects on the wealth of a population as a function of its size and the amount of cash reserves banks are required to hold.  

There are three classes of people in this model: rich, poor, and middle class. The people are represented as colored circles (green = rich, red = poor, blue = middle) on a grid, and they move randomly to adjacent grid cells. If two people are on the same grid cell at the same time, they may decide to trade. The value of goods traded is determined at the time of the transaction and can be either $2 or $5. If the transaction results in a positive gain for either person, then that person deposits the amount in the bank. If either person trades for a loss, then that person attempts to withdraw from their savings to cover the loss. If they don't have enough savings, then they try to cover the loss with a loan from the bank. The bank is required to retain a percentage of all savings as cash, and if that threshold is met then a loan can be made. Otherwise, the bank cannot offer a loan, and the person is unable to trade.

![Bank Reserves Model](/images/bank_reserves_short.mov)  

If you are interested in running the model yourself, you can view instructions [here](https://github.com/charlieroecss/mesa/tree/master/examples/bank_reserves) in the Mesa GitHub examples. If you have trouble, please explore the Mesa [documentation](http://mesa.readthedocs.org/en/latest/) and then reach out to the ProjectMesa Google [group](https://groups.google.com/d/forum/projectmesa).