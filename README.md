## Automated identification of POI errors.

### Inspiration
As a team, we were motivated by the idea of building a real, applicable solution to a service that is currently available to people all over the world, and one that would have the potential to be improved for actual interaction with users through feedback.

### Problem
**HERE Technologies** is a multinational company specialized in mapping technologies and services. It currently allows users to find Points of Interest (POI) in maps for various countries. However, some current issues that can be found in the maps' details are that locations for a few POI are incorrectly configured. Functionality for the features regarding POI can be divided into four possible scenarios:
1. Outdated map data
2. Incorrect road matching
3. Incorrect street categorization
4. Correct matching and categorization (ideal)

### Project functionality
Using provided data, we first identified those Points of Interest that had incorrect matching. Extracting this data, we then used the **HERE Geocoding and Search API** to find the correct coordinates for each POI by matching their address in the API. With the correct coordinates, we then worked on error detection and fixing road matching for these places.

### Project building
We used **python** in **Jupyter Notebook** to work with the provided data and build the program for error detection.
#### Requirements
Python 3.6 or higher (recommended: Python 3.10+)
#### Packages and libraries
* **Pandas:** for data manipulation and analysis, reading CSV files, handling DataFrames, filtering, merging, and transforming tabular data.
* **GeoPandas:** for geospatial data manipulation and analysis, reading GeoJSON files, handling geospatial DataFrames, spatial joins, and creating geometries.
* **Shapely:** for manipulation and analysis of planar geometric objects, calculating centroids, interpolating points, and finding nearest points.
* **Requests:** HTTP requests library used for sending HTTP requests to external APIs (such as the HERE API) and handling responses.
* **NumPy:** for numerical computing, handling missing values, numerical operations, and array manipulations.
* **Random:** used to generate random numbers, assigning random IDs for data correction and simulation.

You can install this libraries via `pip install`

### Challenges
* The use of the HERE platform was not intuitive. Specially considering that the existence of a deprecated HERE Developer platform generated confusion within the team when trying to integrate the API.
* Initially, there were some errors when trying to find matching data between .csv and .json files.
* Some of the provided data was outdated, which made working with it a bit more difficult, specially when trying to use addresses for the API.

### Accomplishments
We were able to work as a team efficiently, making it possible for us to build and complete the project in 24 hours, while also leaving room for areas of improvement. We were able to integrate the API's functionality in the code, which allowed us to find the right coordinates for places that had outdated location data, or just incorrect location placement.

### Learnings
During the making of this project, we learned about:
* HERE Technologies, their global relevance and the ways in which the company works.
* The manipulation and analysis of data frames containing real and extensive information, using python.
* The integration and usage of the HERE Geocoding and Search API for POI data matching and extraction.

### Future improvements
Through the usage and training of an artificial intelligence model, we could be able to use the identification of POI errors to automate the fixing of incorrect location data for POI in any map. Additionally, the enlarging of the data frames that we use for analysis could significantly improve error detection.
