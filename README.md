2013-2015 Baseball playoff appearances vs. Concession prices

List of code files:
_CODE/database.ini - contains SQL queries to run against PostGres Server
_CODE/config.py - contains method for connecting to DB and running SQL queries against it
_CODE/conn_engine.ipynb - contains engine for running DB queries 

Baseball Project 2.ipynb -  old baseball performance research project and data cleanup
Kylie_Graphs.ipynb - new graphs
Resources/attendance_graph.ipynb - more new graphs!

• We hypothesize that teams who win a lot and have bigger stadiums/are in larger metro areas will have lower cost of food and drink in their stadiums. Teams with few wins, smaller stadiums, and smaller metro areas will have higher prices.

	o Teams that made it to the playoffs in 2013-2015:
		- Stadium size/capacity
		- City population where stadium is located
		- Beer prices
		- Team performance (number of times in the playoffs, possibly more time permitting)

	o Data collected from kaggle, data.world, US Census, and https://www.baseball-reference.com/leagues/MLB/misc.shtml.

We used the psycopg2 package and utilized database.ini file to store all SQL tables and our one mega query. The data was painstakingly cleaned throughout the entire process. 

In regards to our hypothesis, we did not see a clear connection between beer prices/concessions and winning or losing teams. It seems there are more factors involved. 
Some points to note and lessons we learned:
 
	•There are a number of factors that go into beer cost at stadiums, but they may have more to do with local tastes than winning performance
	•There may be a connection between attendance and beer costs, but there is a floor for beer prices. With more time we would look more into population, stadium capacity, 	   and perhaps even availability of craft vs. domestic beers
	
	•Biggest challenge was normalizing data and cleaning it (no surprise there)
	•It helps to test affects of every change – sometimes edits made to one table impacted the connection to another
