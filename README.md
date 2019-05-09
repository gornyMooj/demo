# Census Co. Kildare - [demo](https://gornymooj.github.io/demo/)

This short demo shows usage of D3.js in visualization of the change of the population in Co. Kildare. The statistic data was taken from the official website of [Central Statistics Office(CSO)](http://census.ie/), years:
- 1996
- 2002
- 2006
- 2011
- 2016

The data is displayed in the form of the choropleth map representing the number of people living in a given electoral division ([ED](https://en.wikipedia.org/wiki/Electoral_division_(Ireland)) - *the smallest legally defined administrative areas in Ireland for which small area population statistics*). 

Tabular Data
Tabular data was downloaded in the CSV format from the CSO database for each census. The data were merged into the one [CSV table](https://github.com/gornyMooj/demo/blob/gh-pages/census.csv). This process required unification of the schema across all the tables. Manly the work was done manually and some of the steps in data processing were managed using Python scripts. 



