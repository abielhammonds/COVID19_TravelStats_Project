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
    Contains the code for making multiple API calls to collect the CDC COVID data.

COVID19Travel_Create_DataFrames.ipynb
    Contains the code for creating a DataFrame from the CDC and TSA data.

COVID19Travel_Visualizations.ipynb
    Contains the code for creating the visualizations and analyzing the data.
