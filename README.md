# ChicagoCrimeBigDataAnalysis

Data Link: https://catalog.data.gov/dataset/crimes-2001-to-present-398a4
Plotting Graphs: https://plot.ly/create/

The dataset contains approx 12lakhs records having 22 columns. Analysis is done using R programming in RStudio.
Packages Required:
sqldf and dependencies which it requires.

Running SQL Queries after installing packages.

library(sqldf)
Load the dependencies too:- 
## RSQLite, proto, gsubfn etc.

Clean the data first, remove missing values and remove spaces from column names.

After that, whatever you can draw fron the data run sql query for that. 
For eg.

### primarytype_crime = sqldf("Select PrimaryType, count(*) as frequency from CrimeData group by PrimaryType")

This is how the whole analysis is performed.

Saving the results in csv file and uploading the data in plotly library and make the graphs.
