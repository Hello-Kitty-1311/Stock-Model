# Stock Price Prediction Model - V1
this is a program i built that tries to predict stock prices. you just run it and type in a stock ticker like tsla or googl and it grabs all the data from the internet.

then you can choose what kind of prediction method you want to use. theres a fast one called xgboost which is pretty good and then a much slower one called lstm which is a neural network that can sometimes be more accurate. or you can use both.

## Why i made this ipynb

* i started trading stocks and i was really bad at it tbh
* i was losing money just guessing so i figured i could code something to help
* i wanted more than a graph i wanted something to give me an actual opinion
* thats why i made the recommendation part that gives you a percentage score
* it was more about building a tool to help me stop making dumb choices than building a perfect system

## How i made it

* i used a thing called yfinance to grab all the historical stock data
* then i calculated a bunch of technical indicators like rsi and macd becuase i thought more data would be better
* for the predictions i used two main things
* one is an xgboost ensemble which is basically a few smart models that vote on the answer
* the other is an lstm neural network which is good with time but takes forever to train
* i used a library called plotly to make the interactive graphs
* at the end i added some code to save the trained models so i dont have to run the whole training process every time

## struggles and what i have learned

* getting the data ready for the lstm model was a nightmare it's so picky about the format
* training the lstm took ages my laptop fan would go crazy for like an hour each time
* the fanciest model isnt always the best i learned. the faster one was almost as good
* the worst struggle was a super weird error when i tried to save the model i had to install an older version of a library called scipy which took forever to figure out
* i learned that your tools can be the problem not just you're code
* also learned predicting the market is basically impossible but making the tool taught me a ton about machine learning and that most of the work is just cleaning data

## usage of AI

* Error Lens : finds error in realtime
* Amazon Q Cli : real time code suggestion and explains error
* ChatGPT and Claude : solves bigger porblems

## what you can expect in V2

* this 1st version has a drawback of large runtime nearly { 40 mins }
* the prediction is not that accurate so i need to improve its accuracy
* cannot be used on webpage as backend coz no user will wait for 40 mins to get result so a lite webpage version is coming soon.
