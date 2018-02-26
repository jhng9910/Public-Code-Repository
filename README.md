# Public-Code-Repository

You’re logged in to a production system that holds archived server logs. The logs are stored in nested directories by year and month. 
There is one log file per day:

 |-- 2016
 |   |-- 2016-01
 |   |   |-- 2016-01-01.log
 |   |   |-- 2016-01-02.log
 |   |   |-- 2016-01-03.log
...
 |   |   |-- 2016-01-31.log
 |   |-- 2016-02
 |   |   |-- 2016-02-01.log
 |   |   |-- 2016-02-02.log
 |   |   |-- 2016-02-03.log
...
etc
Each line in the log is one HTTP request, with an excerpt from 2017/2017-02/2017-02-04.log included below:

2017-02-04T23:03:13 "GET http://myfakesite.com:80/home HTTP/1.1"
2017-02-04T23:04:21 "GET http://myfakesite.com:80/secretpath?with=arguments HTTP/1.1"
2017-02-04T23:05:45 "GET http://myfakesite.com:80/api HTTP/1.1"
You recently launched an /api endpoint and are curious how many days it has been accessed. Bearing in mind that it is a one-off task,
how do you count the number of days where the endpoint was hit? 
