# San Diego Accident Analysis

Authors: Huy Trinh, Jianming Geng, Yacun Wang<br>
June 16th, 2023

### Data

#### Raw Data Sources

We are using San Diego Data Portal for our raw data, including information on the accidents, Get-It-Done Reports, and roads:
- [Traffic Collision Records](https://data.sandiego.gov/datasets/police-collisions/)
- [Vehicles and People Involved in Accidents](https://data.sandiego.gov/datasets/police-collisions-details/)
- [Get It Done Requests](https://data.sandiego.gov/datasets/get-it-done-311/)
- [Roads](https://data.sandiego.gov/datasets/roads-lines/)
- [San Diego City Boundary](https://data.sandiego.gov/datasets/san-diego-boundary/)

Running data preprocessing requires Python GIS packages and an ArcGIS Online Account with ESRI credits, so we don't recommend running the preprocessing as we have prepared processed data.

#### Processed Data

All processed data are created and stored under the [Shared Google Drive](https://drive.google.com/drive/folders/1wpifXxdnxIrisuvbvu8xhulW7McIjEPo?usp=sharing). Download these data and store them in the `data` directory, as well as the `"neo4j-docker - GDS"/db/import` directory.
