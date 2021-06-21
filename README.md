# Seoul Public Bike(Ttareungyi) Real-Time Map

<br/>
<br/>
## Objective


The number of public bike rental stations in Seoul exceeds 1,500. Rather than clicking dozens of nearby rental stations one by one, if service users can see maps with icons identified by colours according to the number of bikes, they may be able to solve their small inconvenience.
Its objective is to increase user convenience by establishing an Html map to make it easier to check the real-time number of bicycles available at the Seoul public bike rental station by colour.


<br/>
<br/>
## Contents

The project consisted of the following steps:

1. Data collection
  * Use [API](http://data.seoul.go.kr/dataList/OA-15493/A/1/datasetView.do) of Real-time rental information of public bike in Seoul from Seoul public data center
  * Description of dataset
 
| No |       Field       |                  Description                  |
|:--:|:-----------------:|:---------------------------------------------:|
|    | list_total_count  | Total number of data (output on normal query) |
|    | RESULT.CODE       | Request result code                           |
|    | RESULT.MESSAGE    | Request result message                        |
|  1 | rackTotCnt        | Number of dock                                |
|  2 | stationName       | Name of station                               |
|  3 | parkingBikeTotCnt | Total of parking                              |
|  4 | shared            | Dock rate                                     |
|  5 | stationLatitude   | Latitude                                      |
|  6 | stationLongitude  | Longtitude                                    |
|  7 | stationId         | Station ID                                    |
  
2. Data Wrangling
  * Identify null rows in the data frame.
  * Select information

3. Data Visualization
  * Visualize map with the icons of stations
  * Visualize cluster map of station colored by conditions
  * Visualize mini map
<br/>
<br/>
<br/>
You can check out the [results[(https://github.com/E-Song330/Seoul-Public-Bike-Real-Time-Map/blob/3ec6870c00652b1bf99bc60feaee320ac60b373a/Seoul%20Public%20Bike%20Real-time%20Map.md
