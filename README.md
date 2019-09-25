# Uber Ridesharing data in Victoria, Australia .

# Data Cleansing


Exploring and understanding the data is one of the most important parts of the data wrangling
process. You are required to perform both graphical and non-graphical EDA methods to
understand the data first and then find the data problems. You are required to:

● Detect and fix errors 

● Detect and remove outliers 

● Impute the missing values 

As a starting point, here is all we know about the dataset in hand:
The dataset is about Uber Ridesharing data in Victoria, Australia . The description of each data
column is shown in Table 2.
Table 2. Description of the columns


# COLUMN DESCRIPTION

# Id 
A unique id for the journey

# Uber type 
A categorical attribute for the type of the journey namely Uber
pool, Uberx, Uber black. All we know is that the cost of these
types of journeys may be different.

Origin region A categorical attribute representing the region for the origin of the
journey

Destination region A categorical attribute representing the region for the destination
of the journey

Origin latitude Latitude of the origin coming from Nodes.txt file

Origin longitude Longitude of the origin coming from Nodes.txt file

Destination latitude Latitude of the destination coming from Nodes.txt file

Destination longitude Longitude of the destination coming from the nodes.txt file

Journey Distance The shortest path, in meters, between the origin and the
destination with respect to the nodes.txt and the edges.txt files.
Dijkstra algorithm can be used to find the shortest path between two
nodes in a graph. Reading materials can be found here .

Departure date Date of the departure. We know that the price is different on
weekdays compared to weekends.

Departure time Time of the departure. We know that the Uber company has a
specific rule to define a discrete number for morning (i.e. 0)
(6:00:00 - 11:59:59), afternoon (i.e. 1) (12:00:00 - 20:59:59), and
night (i.e. 2) (21:00 - 5:59:59) to calculate the fare.

Travel time Travel time (i.e., duration) of the journey in seconds. Note that
road types have their own speed limit in the edges.txt file and the
car always travel with the exact speed limit.

Arrival time The time of the arrival

Fare$ The fare of the journey. We know that the fare has a linear
relation with some of the attributes of the dataset.

