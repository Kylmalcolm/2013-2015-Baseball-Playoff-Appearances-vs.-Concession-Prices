<h1> 2013-2015 Baseball Playoff Appearances vs. Concession Prices </h1>

Copied from original repo: https://github.com/eerofeeva/return_of_the_Baseball_Madness which has the commit history attached.

My main focus for this project was data clean up, creating graphs, and written analysis.

![image](https://user-images.githubusercontent.com/70925750/112413035-8287ae80-8ced-11eb-97e0-a6bb8ed91ef2.png)

<b> List of files:</b>
_CODE/database.ini - contains SQL queries to run against PostGres Server
_CODE/config.py - contains method for connecting to DB and running SQL queries against it
_CODE/conn_engine.ipynb - contains engine for running DB queries 
Baseball Project 2.ipynb -  prior baseball performance research project and data cleanup
Kylie_Graphs.ipynb - new graphs
Resources/attendance_graph.ipynb - attendance graphs

![image](https://user-images.githubusercontent.com/70925750/112413081-959a7e80-8ced-11eb-8958-873e9070263e.png)

We hypothesized that teams who win a lot and have bigger stadiums/are in larger metro areas will have lower cost of food and drink in their stadiums. Teams with few wins, smaller stadiums, and smaller metro areas will have higher prices.

The data was collected from kaggle, data.world, US Census, and https://www.baseball-reference.com/leagues/MLB/misc.shtml.

We used the psycopg2 package and utilized database.ini file to store all SQL tables and our one mega query. The data was painstakingly cleaned throughout the entire process. 

<b> In regards to our hypothesis, we did not see a clear connection between beer prices/concessions and winning or losing teams. It seems there are more factors involved. 
Some points to note and lessons we learned: </b>
 
There are a number of factors that go into beer cost at stadiums, but they may have more to do with local tastes and markets than winning performance

There may be a connection between attendance and beer costs, but there is a floor for beer prices. With more time we would look more into population, stadium capacity, and perhaps even availability of craft vs. domestic beers
	
The biggest challenge was normalizing data and cleaning it

It helps to test affects of every change – sometimes edits made to one table impacted the connection to another
