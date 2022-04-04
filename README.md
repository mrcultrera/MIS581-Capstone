# MIS581 Capstone
 
This project analyzes historical pricing data from large-cap stocks, indices, and cryptocurrencies.  The purpose of the project is to understand the potential relationship between common technical analysis ("TA") indicators and future price movements of these tradeable assets.

The perspective of the project is that of Robinhood.  Robinhood's customer base is primarily young and inexperienced investors.  These investors are likely to come across assertive and overly confident social media influencers proclaiming the certainty of TA.  Robinhood can help protect their users, reduce criticism from the financial industry, and potentially offer a unique service to their customers by adopting and publishing a clear and unbiased analysis of TA.

The project contains three sections: 
The first section focuses on moving average crossover strategies which provice oscillating buy and sell signals.  This approach is compared with a simple buy and hold strategy.  

The second section identifies three day periods of consistently increasing/decreasing price and volume resulting in five buckets: PriceUp_VolumeUp, PriceUp_VolumeDown, PriceDown_VolumeUp, PriceDown_VolumeDown, Mixed_No Trend.  After these trends are identified a multivariable linear regression analysis is performed to evaluate any relationships with future price fluctations.  

The third section is focues on chart patterns which are common patterns seen when viewing a pricing chart over time.  TA advocates will claim that these common chart patterns are frequently followed by a bullish or bearish price trend.  A neural network was trained on synthesized chart pattern pricing charts.  The six chart patterns considered are the following: Double Top, Double Bottom, Head and Shoulders, Inverted Head and Shoulders, Cup and Handle, and Inverted Cup and Handle.  After the neural models were developed, the historical pricing data was mined for pricing charts in 3 day iterations with a timeframe of 20 days, 35 days, and 50 days.  These generated pricing charts were then input into the neural network models for confirmation of these patterns.  After records were identified by these chart patterns, a multivariable linear regression analysis was done to evaluate their relationship with future pricing changes.
