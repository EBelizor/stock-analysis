# stock-analysis

## Overview of Projects 

In this challenge we are helping Steve as he assists his parents in managing their portfolio. Steve’s parents are big believers in green energy, however Steve’s parents have made all of their investments into the stock “DQ”. We ran the analysis by year and were able to truly analyze the green stocks to see the value that Steve’s parents were getting out of their investments. The VBA script that we ran was able to analyze the stock trends by year accurately. While our stock analysis ran well, Steve was thinking bigger picture, and Steve wanted to see the code scale in order to handle larger data sets. Thankfully for us we can simply refractor the code to handle far more stocks.

## Results 
When we analyze the stocks we see a stark difference in the performance of these stocks by just looking at the colors of our conditional formatting for our returns. When we look at 2017 we see a lot of green (positive returns), in terms of our returns meaning that this was a great year for “green” stocks or stocks in general. “DQ” easily  outperformed all of the green stocks that were in our data set as it yielded a whopping 199.4% return rate. However, the following year it performed the most poorly yielding a concerning -62.6% return rate.

Our initial code relied heavily on nested loops, and while nested loops are very effective, the code can be very inefficient when it comes to the potential of expanding our data set. Nested loops run iterations of other loops within the main loop, and while the code runs perfectly fine the issues start to arise when we increase our data set. Our initial analysis ran the data in .25 seconds for 2017 and 2018. 

![](stock-analyis/resources/origin_code)


Our refractored code was able to dramitically decrease the run time to .053 seconds. This difference comes from us using arrays coupled with for loops to alleviate the stress of nested loops in our code. Using arrays allows us to store values of similar variable types so that we can command VBA to lookbak on that array and any number that is linked to a vallue in that array will be pulled for that specific loop! Doing so allows for us to 


## Summary 
  
  While a .20 second difference might not seem significant to you now, it can make a world of a difference as the data expands because that 20 second gap can easily become a 2 minute gap and more in our analysis. That dramatic difference comes simply from what we are telling our software to do. A nested loop means that we are telling our system to run code "in and out and in and out" between our main loop and the loops that lie within them. In a nested loop we see that our for loops that are within other loops are ran by their parameters along with being multiplied by every outside loops parameters as well. As you can imagine, if you run a few "for" statemtents with thousands in their parameters we will get very very large numbers. However, the use of arrays to make our code commit to memory allows us to run our data in a more chain like fashion which saves a lot of time. 
  
  Now refactoring code is not all positive, this can take a lot of time to perfect. When you mess with one script of code you run the risk of changing dependent parts of other code, which can be time exhaustive. Refactoring code takes understanding of your commands, you must know what you can change and what you cannot, it is never a good idea to go into a refactoring process and not understand the previous code. 
  
  ### Conlusion
  
  Taking the ability to save countless time into effect, it would seem that changing our code might be a no brainer. It turns out Refactoring code is always situational. For Steve it makes perfect sense because he wants to reuse the code to expand his analysis into many other stocks. If an individual or organization does not plan to run an analysis often or even expand their analysis, I would not recommend refactoring. In most cases we will be running data analysis over and over again, so it makes sense for us to refactor to speed up. Data is constantly changing and so our code should evolve with it, while refactoring can take time, the evidence shows that it can yield far greater returns in the future. 
