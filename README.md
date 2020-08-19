# Portfolio-construction-and-optimization-using-sentiment-analysis-of-10k-documents

The 10k filings of few companies in technology and finance sector were extracted . 
Next , the sentiments of the 10ks were found using Loughran Mcdonald sentiment words by creating a bag of words matrix for each sentiment for all documents of a particular company and Jaccard Similarity of neighbouring rows in the matrix was calculated . 
The sentiment with the highest Jaccard similarity score for a document was taken as the sentiment of the document and the corresponding Jaccard similaity score as sentiment score . 
Nest , using these scores and the yearly returns and volatility , a regression model was formed to calculate the return and volatility for the year 2015-16. The aim was to explore whether the sentiment of 10k filings for a particular year help us forecast the return and volatility we can get the next year .
Ex : 10k filings which were filed during Jan 2015 used to forecast the return for 2015-16. 

Next , using these predicted return and volatility for each company , a portfolio was created and also optimized weights for each stock were calculated . 
This portfolio was backtested on Quantopian platform but the net return turned negative , even lower than S&P 500 (which had negative growth too in 2015-16) . Although this cannot be used as an effective investment strategy , it was just an attempt to study the correlation that 10k documents can have with annual returns and annual volatility . This opens the door for further research into other factors affecting stock market returns and those which can help in formulating investment strategies.
