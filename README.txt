The nature of the project was using neural networks and Fama-French 5-factor model to give predictions of stock prices.

The approach of the study was simple and there were a lot to be improved.
1. As we all know, price data is non-static and it's not normally distributed. Therefore, in a time-series based analysis, it's better to use return instead of price.
2. The data source chosen in the project was yfinance API which provides data from Yahoo Finance. However, this is not a data source with the highest quality. It may be optimal to switch to other sources.
3. Deep Learning models may be too complex and have too high of variance for the size of data.

After acquiring the data from yfinance and Kenneth Data Library, I combined them together and did some simple cleaning. The data was then fed to the model through a generator function.
The training and tunning process can be seen in the jupyter notebook file. And the prediction result was at the very end.

The accuracy of the prediction was limited. But compare to the baseline model, which was a moving average, LSTM is still outperforming.
