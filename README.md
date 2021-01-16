# NYC Restaurants Health Inspections

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

There is only one library to install, beyond the Anaconda distribution of Python: Folium.

```$ pip install folium```

The code should run with no issues using Python versions 3.*.

## Project Motivation<a name="motivation"></a>

Since 2010, New York City has required restaurants to post letter grades that correspond to scores received from sanitary inspections. 
Inspections detect potential health violations, and each violation has a number of points attached to it depending of its severity. 
A total inspection score of 0 to 13 is an A, 14 to 27 points is a B, and 28 or more points is a C. Grade cards must be posted where they can easily be seen by people passing by. Two subsequent C grades, will result into a temporary closure.

For this project, I use the results of NYC Sanitary Inspections from December 2020 to June 2014.
The data is regularly updated and available on NYC Open Data website ans can be found [here](https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/43nn-pn8j).

I wanted to understand, the following:

1. Are there some areas of NYC where there are more less safe restaurants than others?
2. Are there some type of cuisines which seem less safe than others?
3. Are there some time of the year when the risk could increase?
4. What are the most frequent type of issues detected during inspections?
5. Do previous grades and previous inspection results of an establishment matter ?
6. Finally, would it be possible to build a model to detect the establishments not having the best A grade ?

## File Descriptions <a name="files"></a>

There is one notebook available here to showcase work related to the above questions. Markdown cells and comments were used to assist in walking through the thought process for individual steps.

There are three .csv files:
1. DOHMH_New_York_City_Restaurant_Inspection_Results- part 1 and 2. Had to split the file to be able to push to Github. This is the database retrieved from NYC Open Data as of 16th December 2020
2. RestaurantInspectionDataDictionary_09242018- dictionnary of the database retrieved from NYC Open Data

One .doc file -About_NYC_Restaurant_Inspection_Data_on_NYC_OpenData_092418- the documentation attached to the database and retrieved from NYC Open Data

Two .pdf files giving more background on the inspection process

One .geojson file, containing boundaries for NYC zip codes. It can be found [here](https://data.beta.nyc/en/dataset/nyc-zip-code-tabulation-areas/resource/894e9162-871c-4552-a09c-c6915d8783fb?inner_span=True)

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://mrnpetel.medium.com/nyc-restaurants-how-to-choose-safely-9d5112998e91).

## Acknowledgements<a name="licensing"></a>

Must give credit to NYC Health Department for the data.
