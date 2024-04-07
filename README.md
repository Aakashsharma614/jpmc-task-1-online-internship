# jpmc-task-1-online-internship
this is my first task of jpmc virtual internship.
Here is the background information on our task

we’ve been asked to assist with some development to add a chart to a trader’s dashboard allowing them to better identify under/over-valued stocks.

The trader would like to be able to monitor two historically correlated stocks and be able to visualize when the correlation between the two weakens (i.e. one stock moves proportionally more than the historical correlation would imply). This could indicate a potential trade strategy to simultaneously buy the relatively underperforming stock and sell the relatively outperforming stock. Assuming the two prices subsequently converge, the trade should be profitable.

Most data visualization for our traders is built on JPMorgan Chase's Perspective data visualization software, which is now open source.

Before implementing this request using perspective, first you’ll need to interface with the relevant financial data feed and make the necessary adjustments to facilitate the monitoring of potential trade opportunities.

Understanding the finance and trading part is not required.

Being familiar with python scripting language and command line basics is not required as you will be guided in this exercise

For the first module of this project will we need to accomplish the following:


1.Set up your system by downloading the necessary repository, files, tools and dependencies

2.Fix the broken client datafeed script in the repository by making the required adjustments to it.

3.Generate a patch file of the changes you made

4.Bonus task: Add unit tests in the test script in the repository.

Step1:Set up your system
how to setup your enviroment for this task Click Here
Step2:Fixing the broken clinet datafeed script
Before fixing the client code we need to know what the code is actually doing there is 3 python file in the task

Server3.py
Client3.py
Client_test.py
So let's find what the file is doing

Server3.py
This program is used to serve a stack market data to client by using HttpServer . It read the data from the excel file (test.excel) and send the data to client3.py to know more read the source code

client3.py
This program get the data from server3.py and calculate the trade price and ratio of two stack price.
