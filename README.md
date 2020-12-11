# PLSC31101-finalproject-YukiWang
# Short Description
Scrap and download data from the website of the IMF and the World Bank. Clean the data using functions like select, filter, arrange, and mutate. Make some calculation and create new data frames for plotting. Merge different dataframes to a new one for regression.

# Dependencies
RStudio Version 1.3.1093.

library(XML)

library(tidyverse)

library(rvest)

library(lubridate)

library(readxl)

library(cowplot)

library(ggplot2)

library(stringr)

library(stargazer)

library(httr)

library(rjson)

# Files
Code/

1. final project - Yuki Wang.Rmd: Data collection,pre-processing,visualization and analysis.

2. appendix.Rmd: Webscraping from the IMF news section which is a dynamic website (this part is not included in the formal project).

Data/

1. votes.csv: Contains data scraped from the "IMF Members' Quotas and Voting Power, and IMF Board of Governors" https://www.imf.org/external/np/sec/memdir/members.aspx#Z. Includes all IMF member states' vote shares in 2016.

2. votes.xlsx: The excel version of the votes.csv

3. quotas.xlsx: Updated IMF Quota, available here: https://www.imf.org/external/np/fin/quotas/2018/0818.htm

*cal_before: calculated quota shares before the first round of reform (2006) 

*cal_review: calculated quota shares after the first round of reform (2008)

*cal_previous: calculated quota shares after the second round of reform (2012)

*cal_current: calculated quota shares after the third round of reform (2016)

4. arrangement.xlsx: IMF Monitoring of Fund Arrangements (MONA) Database Country-level data, available here:https://www.imf.org/external/np/pdr/mona/Country.aspx

5. CV.xlsx: World Bank Open Data, available here: https://data.worldbank.org/indicator with observations of year 2006 for the following variables:

*gdpPercap:GDP per capita (current US$)

*reserve_debt:International reserves to total external debt stocks

*FDI:Foreign direct investment, net inflows (BoP, current US$)

*IMFcredit:Use of IMF Credit: Data related to the operations of the IMF are provided by the IMF Treasurer’s Department

*Account_balance:Current account balance (BoP, current US$)


Results/

1. plot1.png: Graphs the average quotas and growth rate during the reforms of main countries.

2. plot2.png: Graphs the quota growth rate by quota during the refroms of all countries.

3. plot3.png: Graphs the quota growth rate and quotas of greatpowers before and after the reform.

4. regression-table1.txt: Summarizes the results of OLS regression, modelling votes and conditionality on a number of covariates.


# More Information

Yuki Wang

wangyuqi@uchicago.edu
