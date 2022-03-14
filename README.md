# VBAChallenge
VBA Stock Challenge for Data Science Boot Camp


# Objective : Improve Efficiency of Stock Analysis

Our client, Steve, loves the workbook prepared for him. At the click of a button, he can analyze an entire dataset. Now, to do a little more research for his parents, he wants to expand the dataset to include the entire stock market over the last few years. Although the code works well for a dozen stocks, it might not work as well for thousands of stocks. And if it does, it may take a long time to execute.

In order to all Steve to scale his reasearch up to a larger selection of stocks, the objective is to refactor the code.  *Refactoring* is a coding process of streamlining process in code in order to improve efficiency.  In order to test if efficiency has been improved, we will evaluate the time it takes for calculations to run to completion.  We will compare the rates from the original code and the refactored code. 

# Results

The original calculations were conducted using nested loops and checking for ticker symbols in each row.  This process was successful and generated calculations for each stock ticker.  

![AllStocksCode](https://user-images.githubusercontent.com/98054953/158203209-418df9cd-956a-4af1-b067-f851069246a5.png)

Screeenshots of the timer message were captured to show the elapsed time for each year using the original code. 

<img width = "258" alt="2017TimewithAllStocks" src="https://user-images.githubusercontent.com/98054953/158035849-f6a030f1-aca4-43bd-bf1b-c7e987f8613b.png"> <img width="258" alt="2018TimewithAllStocks" src="https://user-images.githubusercontent.com/98054953/158035754-e9093bc2-e539-4567-a340-0b003c258ae0.png"> 

The code was refactored to utilie and index and, therefore, reduce the number of times the code has to scan each line for the ticker and corresponding prices and volumes. The updated code is shown below. 

![RefractedCode](https://user-images.githubusercontent.com/98054953/158204058-9ef5f0b8-4701-4e83-a4d0-3f77684daec7.png)

The updated code was more efficient, resulting in runtimes that were faster (78% faster for 2018 analysis and 77% faster for 2017 analysis). 

<img width="257" alt="VBA_Challenge_2017" src="https://user-images.githubusercontent.com/98054953/158204227-d94cbc97-de4a-4bf5-a050-c90689cd8569.png"> <img width="253" alt="VBA_Challenge_2018" src="https://user-images.githubusercontent.com/98054953/158204229-84f1d7f2-c3fd-48d4-b2c0-b1f0bc4d6540.png">

The results were color coded for easy interpretation by Steve.  At a glance he can see which stocks improved (green) and which stocks decreased (red). 

<img width="267" alt="AllStock2017Output" src="https://user-images.githubusercontent.com/98054953/158035813-65f9cdcb-d2dd-44b9-a11f-edb5953458c5.png"> <img width="279" alt="AllStock2018Output" src="https://user-images.githubusercontent.com/98054953/158206529-8f023da1-1899-4248-a55d-3f229a88f8dc.png">



