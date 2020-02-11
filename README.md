# IoT-application
«Design and implementation of an IoT platform for analysis of weather conditions»

Use of the node-red node«openweathermap»

Visualization  in  real  time  using  node-red  the  graphs  for  (temperature,  time),  (humidity,  time), 
(atmospheric pressure, time) for the location of Kastoria,Greece

Display every 2 hours a small description for the current weather conditions in Kastoria

From the openweathermap.org we receive in node-red the weather widget for real time weather conditions and display them in Dashboard.

From the interface https://openweathermap.org/forecast5 receive the data of the last 5 days grouped per 3 hours and store them in a database(SQLite).

These data in JSON format are for the  temperature, the  sea level,the  humidity and  the  atmospheric  pressure. 
For storing them,we use in node-red the«litedb» node.

Using the nodes «function» and «litedb» of node-red we develop a program in javascript that receive these values from the database and it compute the daily average for the temperature, the sea level, the humidity and 
the atmospheric pressur eand then display the average in node-red’s UI in a graph or in a table (you choose).
Finally, we compute the maximum and minimum values per day for the last 5 days and display them in a graph in node-red.
