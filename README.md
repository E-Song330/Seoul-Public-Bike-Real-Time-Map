# Seoul Public Bike(Ttareungyi) Real-Time Map

<br/>
<br/>

## Objective


The number of public bike rental stations in Seoul exceeds 1,500. Rather than clicking dozens of nearby rental stations one by one, if service users can see maps with icons identified by colours according to the number of bikes, they may be able to solve their small inconvenience.
Its objective is to increase user convenience by establishing an Html map to make it easier to check the real-time number of bicycles available at the Seoul public bike rental station by colour.
<br/><br/>
 * Actual serviced map
<img width="300" alt="스크린샷 2021-06-21 19 13 04" src="https://user-images.githubusercontent.com/85876717/122803978-99777600-d2c7-11eb-8fb2-69f66845daa9.png">
<br/>

It's a current serviced map at the web page of [Seoul bike](https://www.bikeseoul.com/app/station/moveStationRealtimeStatus.do?searchValue=서울&searchType=)

<br/>

There are too many bike stations to check availability while clicking one by one, because of there is no division by quantity, but just by bike models.
<br/>
<br/>

<img width="300" alt="스크린샷 2021-06-21 19 13 54" src="https://user-images.githubusercontent.com/85876717/122803990-9bd9d000-d2c7-11eb-83f3-c97cfc60d290.png">
<br/>
You can see that there is no available bike only when you zoom in to specific station.
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


## Stack

Jupyter notebook, ```folium```,```pandas``` etc.

<br/>
<br/>
<br/>

You can check out the [results](https://github.com/E-Song330/Seoul-Public-Bike-Real-Time-Map/blob/3ec6870c00652b1bf99bc60feaee320ac60b373a/Seoul%20Public%20Bike%20Real-time%20Map.md)
