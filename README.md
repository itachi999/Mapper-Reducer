# Hadoop Mapper and Reducer python program

To get the count of each vehical involved in the accident run the below commands

<b>data is located at /data/nyc/nyc-traffic.csv</b>

run these commands

<b>hadoop jar /usr/hdp/2.6.3.0-235/hadoop-mapreduce/hadoop-streaming-2.7.3.2.6.3.0-235.jar
-file /home/gantihk/mapper.py -mapper /home/gantihk/mapper.py
-file /home/gantihk/reducer.py -reducer /home/gantihk/reducer.py
-input /data/nyc/nyc-traffic.csv -output /user/gantihk/final1-output</b>

output is located at /user/gantihk/final1-output

to view the output run the commands below

<b>hadoop dfs -ls /user/gantihk/cloudhw4-output

hadoop dfs -cat /user/gantihk/cloudhw4-output/part-00000</b>


<h2>output</h2>

AMBULANCE       3713

BICYCLE 24153

BUS     25871

FIRE TRUCK      1333

LARGE COM VEH(6 OR MORE TIRES)  27981

LIVERY VEHICLE  17775

MOTORCYCLE      10029

OTHER   51360

PASSENGER VEHICLE       1005163

PEDICAB 123

PICK-UP TRUCK   26281

SCOOTER 534

SMALL COM VEH(4 TIRES)  30048

SPORT UTILITY / STATION WAGON   363210

TAXI    63892

UNKNOWN 105481

VAN     51666
