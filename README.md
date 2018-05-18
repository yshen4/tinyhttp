# tinyhttp
A tiny http client API written in c++ with minimum dependency

# Why?
There are different http library in the market, which takes advantages of existing works from other developers. However, when we cut short the time to deliver, the dependency on those libraries may grow out of control. On the other hand, many enterprises have their policies to prevent developers using 3rd party code without approval. 

Many times, we just need some simple functions, such as send a request, and parse the response for status, headers, and some data in simple json format. Why can we have a simple one? This repository is for this purpose. 

# parts

I organize the code in 3 parts: 
- tinysock: to send and read data from a socket;
- tinyconnpool: to manage tinysock connection pool;
- tinyhttp: use tinyconnpool for http: GET, PUT, POST, and DELETE
