## Random but not so random strategy
I try to figure out an original and funny portfolio allocation strategy. The goal of our strategy is to randomize a part of the portfolio allocation process. 

### First step :

I use a set of 31 company available in on a given data frame and compute an adjusted sharp ratio. The adjusted Sharp ratio formula is the following SR=   (average return)/(average volatility) , the aim is to try to capture the 10 best adjusted Sharp Ratio we compute in order to create an initial portfolio of 10 stocks.

### Second step :

Let’s set an equally weighted portfolio with the 10th  stocks we choose from the initial data frame. 

### Third step : 

We give each stock a number from one to ten, we then generate a random number every month in order to choose one lucky stock that will receive 9% weight taken from the other stocks (1% from each stock). However, the lucky chosen stock shouldn’t have less than -1% return the last month, if it doesn’t fulfil the condition we generate a new random number. If every stock has a negative return we go forward to the next month. 

### Fourth step :

We then compute the return and the sharp ratio of the portfolio. The funny aspect about this strategy is that no investor have the same return curve nor the sharp ratio and VaR. 
