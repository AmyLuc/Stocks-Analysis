# Overview #

This project was meant to quickly collect data on yearly stock returns, then  clearly display the data for ease of interpretation. The code could quickly and easily be modified to interpret other stock-related data sets, so long as the data is organized by ticker name.

Please be sure to enable macros upon request. You do not need to update the spread sheet if asked.

---

## Summary of Analysis ##


Run and ENPH were the only stocks that had a positive return in both 2017 and 2018. All the other stock options had a negative return for the year 2018. However, run only had a 5.55% increase in 2017, when ENPH had a 129.52% increase in 2017. In 2018, ENPH maintained a 81.92% increase while RUN performed similarly well with 83.95% increase in return. Given that ENPH had a more consistent increase in return for both years, I would recommend that the client direct his parents towards investing in ENPH.

<img width="559" alt="Original-All-Stocks-Analysis-2017" src="https://user-images.githubusercontent.com/91698325/144931343-551eec4e-89d7-4535-bde2-2579fb0ec1d2.PNG">
<img width="557" alt="Original-All-Stocks-Analysis-2018" src="https://user-images.githubusercontent.com/91698325/144931357-d7c4d48b-220f-49fc-b5fb-947e75e86c06.PNG">


  
---

## Original VS Refactored Code ##

The original code with the nested loops was ultimately much faster than the refactored code that only loops through the data once. I don't know why this is, but it may be reversed should the data pool be larger. It may be that the refactored code is only slower with relatively smaller selections of data. 

In general, nested loops take more time than a For Loop that only iterates through the data  because the number of insitances that the computer iterates throught the code is multiplied by however many times a nested loop loops. While the refactored code loops through the data once for each row, the original code loops through once for each row multiplied by 11 due to the nested For loop.

---

### Time Stamps ###
Bellow are screenshots of the message box and printed message that displays how long the original code ran for:




#### Original code 2017 ####

<img width="251" alt="Original-2017-timestamp-msgbox" src="https://user-images.githubusercontent.com/91698325/144931142-8380a475-f2d2-42a1-8b61-69e915dc238b.PNG">

<img width="188" alt="Original-print-timestamp-2017" src="https://user-images.githubusercontent.com/91698325/144931549-036f4a20-15f9-4cbb-9aa2-b23dcb33aa09.PNG">




#### Original code 2018 ####

<img width="250" alt="Original-2018-timestamp-msgbox" src="https://user-images.githubusercontent.com/91698325/144931131-1f5cf7e4-bab8-4db9-8927-0672353c9f67.PNG">

<img width="185" alt="Original-print-timestamp-2018" src="https://user-images.githubusercontent.com/91698325/144931555-d3bc4c79-ff07-4117-9197-bef199ce0def.PNG">






... and the refactored code:
#### Refactored code 2017 ####

<img width="254" alt="Refactored-2017-timestamp-msgbox" src="https://user-images.githubusercontent.com/91698325/144931282-e94ee91b-36c4-49ad-8b02-3b981f7e2e4a.PNG">

<img width="191" alt="Refactored-print-2017-timestamp" src="https://user-images.githubusercontent.com/91698325/144931565-8cf94985-9cf2-4a13-80c1-6ce21f45c382.PNG">




#### Refactored code 2018 ####

<img width="252" alt="Refactored-2018-timestamp-msgbox" src="https://user-images.githubusercontent.com/91698325/144931295-76dc6082-049c-4a67-b63f-d3740a59405b.PNG">

<img width="192" alt="Refactored-print-2018-timestamp" src="https://user-images.githubusercontent.com/91698325/144931573-b54b3e06-ff89-4838-ab0d-9a236c2033f2.PNG">

---

### Quality Test ###
---
The refactored code would not output accurate data  if the data is not organized by stock type. This is due to how I designed the TickerIndex variable to increase. Both the original and the refactored code would be unable to find the return if the data was not grouped by ticker name, but the original would still be able to find the total volume. 

#### Original: ####
<img width="559" alt="Original-All-Stocks-Analysis-2017" src="https://user-images.githubusercontent.com/91698325/144932258-18875ab9-939f-42f2-b662-8550fd59698d.PNG">

#### Refactored: ####
<img width="559" alt="Refactored-All-Stocks-Analysis-2017" src="https://user-images.githubusercontent.com/91698325/144932284-72a41e43-1cc3-4c84-b3ab-cf507a8fd72f.PNG">

#### Original: ####
<img width="557" alt="Original-All-Stocks-Analysis-2018" src="https://user-images.githubusercontent.com/91698325/144933288-6fd677de-d443-4000-8e56-19f4ee009eb1.PNG">

#### Refactored: ####
<img width="559" alt="Refactored-All-Stocks-Analysis-2018" src="https://user-images.githubusercontent.com/91698325/144932339-06bc9b83-a4d0-4d1c-a791-3b485ca3243e.PNG">

Evidently, both codes produce the same output.
