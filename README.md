# st2195_assignment_6

Download the ECB speeches dataset “all_ECB_speeches.csv” [https://www.ecb.europa.eu/press/key/html/downloads.en.html] and the daily EUR/USD reference exchange rate from the _ECB Statistical Data Warehouse_ “data.csv” [https://sdw.ecb.europa.eu/browse.do?node=9691296]. Next, save them as “**speeches.csv**” and “**fx.csv**”. For the speeches.csv, please keep only the “date” and “contents” columns.

Create a **GitHub** repository called “st2195_assignment_6” and include two scripts (one in **Python** and one in **R**) to perform the operations described below, and a README.md file.

1. Load and merge the datasets keeping all information available for the dates in which there is a measurement in “fx.csv”. [1 point]
2. Remove entries with obvious outliers or mistakes, if any. [1.5 points]
3. Handle missing observations for the exchange rate, if any. This should be done replacing any missing exchange rate with the latest information available. Whenever this cannot be done, the relevant entry should be removed entirely from the dataset. [1.5 points]
4. Calculate the exchange rate return. Extend the original dataset with the following variables: “_good_news_” (equal to 1 when the exchange rate return is larger than 0.5 percent, 0 otherwise) and “_bad_news_” (equal to 1 when the exchange rate return is lower than -0.5 percent, 0 otherwise). [1.5 points]
5. Remove the entries for which contents column has NA values. Generate and store in csv the following tables: [1.5 points each]
a. “_good_indicators_” – with the 20 most common words (excluding articles, prepositions and similar connectors) associated with entries wherein “_good_news_” is equal to 1;
b. “bad_indicators” – with the 20 most common words (excluding articles, prepositions and similar connectors) associated with entries wherein “bad_news” is equal to 1;
Any observation from the common words found above?

Note that the original data should not be included in the GitHub repository, but only appropriately described and linked in the readme file.
