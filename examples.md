---
layout: post
title: Examples
permalink: /examples.html
---

# Master's Thesis

Regulating the stock market is a tremendous undertaking, and it is vital to its safety and success. Many new regulatory issues have arisen along with the prevalence of electronic trading. One of these issues is known as maker-taker fees, which are essentially a means for stock exchanges to incentivize traders to offer liquidity at their venue. These fees were initially regulated at the beginning of the rise of electronic trading, but many argue this regulation needs to be updated to keep up with the practices that have evolved regarding the use of the fees. My thesis describes an agent-based model with minimally intelligent traders interacting in an artificial stock market with maker-taker fees. The purpose is to shed light on the effects of maker-taker fees as well as provide insight into the usefulness of agent-based modeling as a supplemental tool for regulatory decision-making. Results from the study show that maker-taker fees positively affect traditional measurements of market quality, and that minimal intelligence is a viable assumption for traders when modelling the stock market as long as a realistic market structure is present. This research aims to be a step toward incorporating agent-based models into exploratory groundwork for regulatory decision-makers at the Securities and Exchange Commission and other financial market regulatory agencies.  

![Price Match](/images/PriceMatch.png) ![Fractal Price](/images/FractalPrice.png)

# Bank Reserves

This is an example of a very simple agent based model designed to explore the effects on the wealth of a population as a function of its size and the amount of cash reserves banks are required to hold.  

There are three classes of people in this model: rich, poor, and middle class. The people are represented as colored circles (green = rich, red = poor, blue = middle) on a grid, and they move randomly to adjacent grid cells. If two people are on the same grid cell at the same time, they may decide to trade. The value of goods traded is determined at the time of the transaction and can be either $2 or $5. If the transaction results in a positive gain for either person, then that person deposits the amount in the bank. If either person trades for a loss, then that person attempts to withdraw from their savings to cover the loss. If they don't have enough savings, then they try to cover the loss with a loan from the bank. The bank is required to retain a percentage of all savings as cash, and if that threshold is met then a loan can be made. Otherwise, the bank cannot offer a loan, and the person is unable to trade.

![Bank Reserves Model](/images/bank_reserves.mov)  

If you are interested in running the model yourself, you can view instructions [here](https://github.com/charlieroecss/mesa/tree/master/examples/bank_reserves) in the Mesa GitHub examples. If you have trouble, please explore the Mesa [documentation](http://mesa.readthedocs.org/en/latest/) and then reach out to the ProjectMesa Google [group](https://groups.google.com/d/forum/projectmesa).