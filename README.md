# Marketing-Mix-Modeling-

Case Study : 
This is a database of a fictitious soft drink company. This is a time series data with vintage from 1/1/2012 to 1/9/2015 and a monthly granularity.

The data dictionary is as follows:

  - Month – Month of activity
  - SalesVol – Volume of Sales in litres
  - TVGRP – TV Gross Rating Points – the number of times an ad is seen
  - Instoreads – Spends on Ads inside the supermarket – posters, signboards, danglers etc.
  - Outdoorads – Spend on ads on billboards, hoardings, bus shelters etc.
  - Promotions – Spends on promotional schemes like discounts, free gift etc. targeting immediate sales
  - Digitalads – Spends on media like Google Search ads / Google Display ads / YouTube / FB / IG / Twitter etc.
  - Price – Average price per 10 litres
  - Comp1TV – Spends by 1st competitor on TV
  - Comp1NP – Spends by 1st competitor on Newspaper
  - Comp2OOH – Spends by 2nd competitor on outdoor advertising
  - Comp2NP – Spends by 2nd competitor on newspapers

  Using your analysis skills, answer the following questions:

  1) Are soda sales afflicted by seasonality?
  2) Is there a trend seen on soda sales?
  3) What are the correlations between volume sales & media advertising (TV/Instoreads/Outdoorads/Digital)?
  4) What is the correlation between price and volume sales?
  5) What is the correlation between sales volume and promotions?
  6) What is the partial correlation between sales and promotions where TV/Instore/Outdoor/Digital have been partialled out?
  7) Which competitor and their media affect our sales the most?

  8) TV GRP measures the number of times an ad is seen amongst an audience. It is a percentage and can exceed 100 as an ad can be seen multiple times by an individual.
      Advertising has two properties:
      1) Carry over effect
      2) Saturation effect
  Using Excel, transform the column TVGRP to create a new column 'Adstock' with the following formula:

      A(t) = L × A(t−1) + g(t)^n / (g(t)^n + k^n)

      A(t) is the adstock at time t, with the L × A(t−1) term being the carry over property.  g(t)^n / (g(t)^n + k^n) incorporates the saturation effect – sinusoidal curve.
      Where:
      - 0 ≤ L ≤ 1
      - n > 0
      - k > 0
    
The solution workbook consists of the following worksheets : 

  - MMM Data - Dataset of digital channels marketing spends and sales for a fictious soda company
  - Seasonality Analysis - Data exploration, analysis to find the seasonality in the sales data
  - Trend Analysis - Exploring Data for Trends in Sales Volume usin Regression model
  - Media Analysis - Exploring Data to find the correlation of sales with different media channels to find the association
  - Price vs SalesVolume - Data exploration, analysis to find the correlation of price and sales volume in the sales data
  - Promotions Alaysis - Data exploration, analysis to find the correlatio between promotions and sales volume 
  - SalesVol Regression -  Regression model for fitting sales volume over different media channels
  - Promotions Regression -  Regression model for fitting Promotions over different media channels
  - Sales vs Promotions - Partial COrrelations between sales volume and promotions, partialling out the media channels
  - Competitor analysis - Correlation analysis to find out the effect of competitior advertisment strategy over sales
  - Adstock Transformation :  Transforming given data for better visibility


