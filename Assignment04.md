## Assignment 04 ##
### Due [Date and Time] ###

#### Use R to Work with CSV Files and ArcGIS ####

*Note - read full assignment instructions before starting*

Download the .zip "Assignment04.zip" and unzip to your local machine into a folder called "Assignment04."
The folder contains a shapefile and CSV of 2017 Missouri Counties.
Using R, add data from the CSV to the shapefile.

### Part One ###

* Set the path and workspace in R to the unzipped folder.
* Open the "MO_County_2017_Poverty.csv" in R.
* Using the poverty data within the CSV file, create a new dataframe that calculates the poverty rate in each county (divide the "BELOW_POVERTY" field by the "FAMILIES" field).
* Create a combined dataframe with the county names ("COUNTY" field) from the CSV and the corresponding poverty rates.
* Rename the columns of the combined dataframe to "COUNTY_NAME" and "PERCENT_POV".

### Part Two ###

* Use the R-ArcGIS Bridge Library to access the "MO_county_2017.shp" shapefile. In the `arc.select()` function, create a R dataframe object with one attribute based on the "NAME" field of the shapefile.
* Don't forget to convert the R dataframe into a spatial points dataframe.
* Add new county name and poverty rate fields to the shp dataframe based on the columns in the combined dataframe from Part One. The new fields in the shp dataframe should be called "CTY_NAME" and "PCT_POV".
* Create a new shapefile with the new county name and poverty rate fields.

### Submit ###

Upload your R code and submit your assignment as "Assignment04.R"
