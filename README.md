# COVID19_TravelStats_Project
An analysis of weekly COVID case numbers compared with weekly TSA traveller counts and a display of trends.

Data sources:

COVID-19 Case Surveillance Public Use Data: 
    https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data/vbim-akqf
    The data was called in using the SODA API link provided.
    This code is saved in the notebook titled: COVID19_API_Calls.ipynb
    
TSA checkpoint travel numbers for 2020 and 2019:
    https://www.tsa.gov/coronavirus/passenger-throughput
    This data was copied into an Excel document and saved on my local machine as a .csv file

Project files:

COVID19_API_Calls.ipynb
    Contains the code for making the API call to collect the CDC COVID data.
    Then case report date is converted to date format.
    Then the COVID data is grouped by case report date, with a count for deaths and hospitalizations.
    Finally, the group data is exported to a .csv file.

COVID19Travel_Create_DataFrames.ipynb
    Contains the code for combining the CDC and TSA data into a single DataFrame.
    Both types of data were called in from .csv files saved on my local machine.
    Dates were converted from objects to date datatypes
    TSA traveler numbers were converted from objects to floats
    The COVID counts (# cases, #deaths, # hospitalizations per day) are integers.

COVID19Travel_Visualizations.ipynb
    Contains the code for creating the visualizations and analyzing the data.
