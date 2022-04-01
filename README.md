# VBA Stocks Analysis

## Project Overview

A recent graduate financial advisor has requested an analysis of green energy stock options from the years 2017 and 2018. A total of 12 different stock options were analyzed for both years. The opening, closing, high, and low values for each option and each day during a year was included in the data set along with the volume traded. The data set contained 3,012 entries for both years. He has also requested that the original VBA script used be refactored to run the analysis faster.

## Analysis Results

The raw data and analysis can be found at: https://github.com/skgolden13/VBA-Stocks-Analysis/blob/main/VBA_Challenge.xlsm.
The "All Stocks Analysis" sheet contains the analysis. The "2017" and "2018" sheets contain the raw data for their respective year.

In 2017 all options had positive returns except for TERP. The top 3 options were DQ, SEDG, and ENPH with returns of 199.4%, 184.5%, and 129.5% respectively. In 2018 only ENPH and RUN had positive returns, 81.9% and 84.0% respectively. Based on these results, the best course of action would be to invest in ENPH. With strong performances in 2017 and 2018 it is the best option out of the 12 options provided.

The original script ran in 1 second for 2017 and in 1.0625 seconds for 2018. Images of both run times can be found at:
  - https://github.com/skgolden13/VBA-Stocks-Analysis/blob/main/Resources/VBA_Base_2017.PNG for 2017.
  - https://github.com/skgolden13/VBA-Stocks-Analysis/blob/main/Resources/VBA_Base_2018.PNG for 2018.

The refactored script ran in 0.1484375 seconds for 2017 and 0.1484375 seconds for 2018. Images of both run times can be found at:
  - https://github.com/skgolden13/VBA-Stocks-Analysis/blob/main/Resources/VBA_Challenge_2017.PNG for 2017.
  - https://github.com/skgolden13/VBA-Stocks-Analysis/blob/main/Resources/VBA_Challenge_2018.PNG for 2018.

## Analysis Summary

Refactoring a script has the benefits of using fewer steps to achieve the same result, using less memory, and improving the script's logic. These benefits reduce the run time for a script. The main drawback of refactoring a script is the amount of time that could potentially be spent reworking the original version.

The original script was simple to write and performed the analysis as requested. The 1 second on average it took for the original script to run isn't horribly slow. This time will increase as the data set gets larger, making the script unreliable for larger analysis. The refactored script ran in 15% of the time the original script did which would allow for significantly larger data sets to be analyzed.

Drawbacks of both script versions include initializing the tickers for the stock options in the script. This works fine for analyzing a few options, but will not be efficient for analyzing more. Having the script loop through the data and search for each unique ticker would be a more efficient method of analysis. It would also be useful for the script to be able to analyze data on a smaller time scale than an entire year. Looking at the data on a monthly or weekly basis would allow more in depth analysis of current market trends. This would provide investors with a more informed decision.
