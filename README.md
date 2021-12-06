# Overview #
---
This project was meant to quickly collect data on yearly stock returns, then  clearly display the data for ease of interpretation. The code could quickly and easily be modified to interpret other stock-related data sets, so long as the data is organized by ticker name.

---
### Summary of Analysis ###
---

Run and ENPH were the only stocks that had a positive return in both 2017 and 2018. All the other stock options had a negative return for the year 2018. However, run only had a 5.55% increase in 2017, when ENPH had a 129.52% increase in 2017. In 2018, ENPH maintained a 81.92% increase while RUN performed similarly well with 83.95% increase in return. Given that ENPH had a more consistent increase in return for both years, I would recommend that the client direct his parents towards investing in ENPH.
  
---

### Original VS Refactored Code ###

The original code with the nested loops was ultimately much faster than the refactored code that only loops through the data once. I don't know why this is, but it may be reversed should the data pool be larger. It may be that the refactored code is only slower with relatively smaller selections of data. 

Additionally, the refactored code would not output accurate data  if the data is not organized by stock type. This is due to how I designed the TickerIndex variable to increase. Both the original and the refactored code would be unable to find the return if the data was not grouped by ticker name, but the original would still be able to find the total volume. 


