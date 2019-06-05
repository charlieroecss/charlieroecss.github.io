---
layout: post
title: Examples
permalink: /examples.html
---

# Bank Reserves

This is an example of a very simple agent based model designed to explore the effects on the wealth of a population as a function of its size and the amount of cash reserves banks are required to hold.  

There are three classes of people in this model: rich, poor, and middle class. The people are represented as colored circles (green = rich, red = poor, blue = middle) on a grid, and they move randomly to adjacent grid cells. If two people are on the same grid cell at the same time, they may decide to trade. The value of goods traded is determined at the time of the transaction and can be either $2 or $5. If the transaction results in a positive gain for either person, then that person deposits the amount in the bank. If either person trades for a loss, then that person attempts to withdraw from their savings to cover the loss. If they don't have enough savings, then they try to cover the loss with a loan from the bank. The bank is required to retain a percentage of all savings as cash, and if that threshold is met then a loan can be made. Otherwise, the bank cannot offer a loan, and the person is unable to trade.

![Bank Reserves Model](/images/bank_reserves.mov)  

If you are interested in running the model yourself, you can view instructions [here](https://github.com/charlieroecss/mesa/tree/master/examples/bank_reserves) in the Mesa GitHub examples. If you have trouble, please explore the Mesa [documentation](http://mesa.readthedocs.org/en/latest/) and then reach out to the ProjectMesa Google [group](https://groups.google.com/d/forum/projectmesa).