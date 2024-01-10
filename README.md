# San Diego Accident Analysis

Authors: Yacun Wang, Jianming Geng, Huy Trinh<br>
June 16th, 2023

### Problem Statement

Improve profitability of an insurance company by understanding patterns and factors contributing to accidents in the city of San Diego.

### Requirements

#### Code Environment

Throughout the analysis we're using Python in Jupyter Notebooks to run data processing, insertion, and analysis. Specific Python packages listed in the notebooks could be downloaded via `pip install <package>`.

#### Databases

We use two databases to store our data:
- PostgreSQL <img width="3%" src="assets/postgresql.png" alt="Logo"> (Relational Database): Version 13+
- Neo4j <img width="7%" src="assets/neo4j.png" alt="Logo"> (Graph Database):
    - Base Kernel: Version 5.7.0
    - Awesome Procedures on Cypher (APOC) Library: Version 5.7.0
    - Graph Data Science (GDS) Library: Version 2.3.7

### Data

#### Raw Data Sources

We are using San Diego Data Portal for our raw data, including information on the accidents, Get-It-Done Reports, and roads:
- [Traffic Collision Records](https://data.sandiego.gov/datasets/police-collisions/)
- [Vehicles and People Involved in Accidents](https://data.sandiego.gov/datasets/police-collisions-details/)
- [San Diego Get-It-Done Requests](https://data.sandiego.gov/datasets/get-it-done-311/)
- [Roads](https://data.sandiego.gov/datasets/roads-lines/)
- [San Diego City Boundary](https://data.sandiego.gov/datasets/san-diego-boundary/)

Running data preprocessing requires Python GIS packages and an ArcGIS Online Account with ESRI credits, so we don't recommend running the preprocessing as we have prepared processed data.

#### Processed Data

All processed data are created and stored under the [Shared Google Drive](https://drive.google.com/drive/folders/1wpifXxdnxIrisuvbvu8xhulW7McIjEPo?usp=sharing). Download these data and store them in the `data` directory, as well as the `"neo4j-docker - GDS"/db/import` directory.

### Analysis Outline

As suggested by the data sources and their relationships, all analysis questions are separated into 4 parts:
1. Accident Information
2. Accident Vehicle Information
3. Accident Road Information
4. Accident Information in Relation to Get-It-Done Reports

### Main Files Outline
```
San-Diego-Accident-Analysis/
├── data/                            <- all processed data files
│   ├── accidents.csv
│   ├── accidents_info.csv
│   ├── roads.csv
│   ├── reports.csv
│   ├── accidents_on_road.csv
│   └── reports_on_road.csv
├── src/                             <- all code
│   ├── preprocessing.ipynb
│   ├── data-loading.ipynb
│   └── data-analysis.ipynb
└── README.md
```

<div style="float:right">
    <img width="25%" src="assets/HDSI.png" alt="Logo">
</div>
