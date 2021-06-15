# Appsilon Assignment with Ships Data

This is an interactive Shiny Application where the user can select a vessel type and name from the drop down list and then view the details of the longest distance the selected ship has covered.
It calculates the shortest distance between 2 points using distHaversine function between Longitude, Latitude values of 2 consecutive observations ordered with the DATETIME field.

Additionally it calculates the duration in which this longest distance is covered.Also the dashboard has useful indicators from dataset which says which country flag the vessel carries and the speed (in knots).
The data is loaded once and can be processed for many different combinations of vessel type and vessel name which helps in better performance.

Challenges:
** Data Load with read_csv is a bit slow.
 Initial load can be improved further with fread(code commented). 
 However shinyapps.io have difficulty with integer64 format and additional 'bit64' package loading to address that lead to masking of many important functions from base and dplyr package. So that performance optimization stands discarded for this version.

Additionally, more map visualizations can be produced to show the end-to-end ship root. 

The file "ships.csv" attached here is a dummy data just to run the code in working state. Actual data has 3102888 rows of data.

Link to the app: https://riyamol-george.shinyapps.io/Appsilon_Test/
