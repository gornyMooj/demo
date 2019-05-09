# Census Co. Kildare - [demo](https://gornymooj.github.io/demo/)

This short demo shows usage of D3.js in visualization of the change of the population in Co. Kildare. The statistic data was taken from the official website of [Central Statistics Office(CSO)](http://census.ie/), years:
- 1996
- 2002
- 2006
- 2011
- 2016

The data is displayed in the form of the choropleth map representing the number of people living in a given electoral division ([ED](https://en.wikipedia.org/wiki/Electoral_division_(Ireland)) - *the smallest legally defined administrative areas in Ireland for which small area population statistics*). 

**Tabular Data**<br/>
Tabular data was downloaded in the CSV format from the CSO database for each census. The data was merged into the one [CSV table](https://github.com/gornyMooj/demo/blob/gh-pages/census.csv). This process required unification of the schema across all the tables. Manly the work was done manually and some of the steps in data processing were managed using Python scripts. 

**Spatial Data**<br/>
The spetial data was dowloaded in the [shapefile](https://en.wikipedia.org/wiki/Shapefile) format from the CSO website and proccessed in QGIS to extract the boundaries only for EDs located in Co. Kildare. Then the shapefile data was converted into the [TopoJSON](https://github.com/topojson/topojson) format using [Geospatial Data Abstraction Library(GDAL)](https://www.gdal.org/). The TopoJson was used because this format reduces file size, it is substantially more compact than GeoJSON, frequently offering a reduction of 80% or more even without simplification.

**Tools used:**<br/>
- D3.js V3
- Bootstrap 3
- QGIS
- GDAL: ogr2ogr
- Python 2.7
- TopoJSON
- CSV
