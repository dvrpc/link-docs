
## My Studies
The My Studies panel shows the results of each analysis. 
All previous studies completed using your account are listed alphabetically, unless they are deleted. 
At the top of the My Studies panel, you can choose to download a CSV summarizng the results of all studies associated with your account. 

Each study shows the results of the estimated connectivity benefit of the anlayzed segments. 
The results show the total number of various attributes connected by low-stress roads or trails, including the project segment, or by connected sidewalks and crosswalks. 
Attributes are defined in the Study Results Definitations section below.


### Study Results Definitions
- **Miles of low-stress islands**: The total mileage of connected low-stress (LTS 1 and 2 in the bicycle analysis) areas, including the drawn or uploaded facilities being analyzed.
- **Total population**: The estimated number of people living in the census tracts touched by the connected areas, as indicated by the ACS 5-year estimates (2017-2021). The polygon highlighting the low-stress areas connected by the proposed facility improvements is the boundary for inclusion in these estimates. If the polygon covers the entire census tract,  all persons living in that tract are counted. If the polygon covers a portion of a census tract, the proportion of the population counted matches the proportion of the tract area covered by the polygon. The population subsets below are calculated using the same method.
- **Disabled Population**: The estimated number of persons with one or more physical and/or mental disabilities living in the area connected by the analyzed project.
- **Ethnic Minorities**: The estimated number of persons identifying themselves as being of Hispanic or Spanish origin living in the area connected by the analyzed project.
- **Female Population**: The estimated number of females living in the area connected by the analyzed project.
- **Foreign-Born Population**: The estimated number of persons born outside of the United States living in the area connected by the analyzed project.
- **Limited English Population**: The estimated number of persons reporting limited english proficiency living in the area connected by the anlayzed project.
- **Low-income Population**: The estimated number of persons in households with an income below 200% of the national poverty level living in the area connected by the analyzed project.
- **Older Adults**: The estimated number of persons age 65 or older living in the area connected by the anlayzed project.
- **Racial Minorities**: The estimated number of residents who identify as one or more racial minorities living in the area connected by the analyzed project.
- **Youth**: The estimated number of persons under the age of 18 living in the area connected by the analyzed project.
- **Nearby Circuit Trails**: Number and status of circuit trails within the area connected by the analyzed project.
- **Jobs**: The estimated number of jobs in the census tracts touched by the connected areas, as indicated by the American Census Bureau’s LODES 8 dataset (2020). The polygon highlighting the low-stress areas connected by the proposed facility improvements is the boundary for inclusion in these estimates. If the polygon covers the entire census tract,  all persons living in that tract are counted. If the polygon covers a portion of a census tract, the proportion of the population counted matches the proportion of the tract area covered by the polygon. 
- **Bicyclist and Pedestrian Crashes in Study Buffer**: Represents crashes from the last 5 years. This datapoint differs slightly from others, as it only represents crashes within the buffer around your study segment, not in all of the proximate low-stress islands. Note that very long segments will not work
for this metric, as this data is pulled from the DVRPC's crash API, and very long GeoJSON URL strings to the crash API are not supported.  
- **Essential Services**: The number of essential service facilities within the area connected by the analyzed project. Essential services include grocery stores, schools, medical facilites, and activity centers for Seniors or Disabled.
- **Rail Stations**: Number and type of rail stations within the area connected by the analyzed project. 
- **Greater than 300 miles of connected low-stress segments**: For areas such as Philadelphia or Trenton, where islands are extremely large. In these cases, islands are constrained to a 15-minute walk/bikeshed (depending on network type). 
This means that all stats are also constrained to this walk/bikeshed, except for mileage of low-stress islands, which is not reduced.

## Study Options

The following options are available at the bottom of each study.

- Delete Study: removes study from your My Studies panel
- Download GeoJSON: downloads spatial file in the geoJSON format, showing the segments associated with the study, the connected low-stress polygons, and the buffer around the study segments used in the analysis. These spatial files can be viewed in ArcGIS, QGIS, or other spatial analysis software for further analysis and map creation. The segments can also be re-uploaded into the Link tool to be reanalyzed in the future.
- View Study: centers the map on the selected study and shows the study segments and connected low-stress polygon.
- Make Study Public toggle: When turned on, a shareable webpage will be created. This page can be shared with others to view the segments, connected low-stress areas, and the connectivity benefit results. Viewers of the shared link are not required to have a LINK account.




