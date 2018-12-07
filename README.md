# Clustering Chicago Public Libraries

*Author: Kunyu He*

*University of Chicago CAPP'20*

## Introduction

In this project, I clustered 80 public libraries in the city of Chicago with NMF, based on the categories of their top five venues nearby. It would be a nice guide for those who would like to spend their days in these libraries, exploring their surroundings, but become tired of staying in only one or few of them over time. Check [this notebook]() to find these clustered libraries and pick up those surrounded by your favorite category of venues, pay them a visit during their hours of operation!


## Data

Information of the public libraries is provided by [Chicago Public Library](https://www.chipublib.org/). You can access the data [here](https://data.cityofchicago.org/Education/Libraries-Locations-Hours-and-Contact-Information/x8fc-8rcq). Variables includes:

|Variable                       | Definitions                                           | Python Data Type |
|-------------------------------|-------------------------------------------------------|-----------------:|
| NAME                          | Library name                                          | string           |
| HOURS OF OPERATION            | Library hours of operation                            | string           |
| CYBERNAVIGATOR                | Whether there are any cyber navigators in the library | string           |
| TEACHER IN THE LIBRARY        | Whether there is a library teacher                    | string           |
| ADDRESS, CITY, STATE, ZIP     | Address,city, state and zip code of the library       | string           |
| PHONE, WEBSITE                | Phone and website of the library                      | string           |
| LOCATION                      | Library geographical coordinates                      | tuple of float   |

Information of the top venues near to (within a range of 500 meters) the public libraries is acquired from [FourSquare API](https://developer.foursquare.com/). You can explore the surroundings of any geographical coordinates of interest with a developer account. Variables include:

|Variable                       | Definitions                                           | Python Data Type |
|-------------------------------|-------------------------------------------------------|-----------------:|
| Venue                         | Venue name                                            | string           |
| Venue Latitude                | Latitude of the venue                                 | float            |
| Venue Longitude               | Longitude of the venue                                | float            |
| Venue Category                | Category of the venue                                 | string           |
