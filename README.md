# COVID19_TravelStats_Project
An analysis of United States COVID case number trends compared with numbers of airline travelers.

# Data sources:

**COVID-19 Case Surveillance Public Use Data:**
    The data was imported using the SODA API link provided on the CDC websites linked here.
    
    https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data/vbim-akqf
       
    This code shows national case counts and is saved in the notebook titled: COVID19_API_Calls.ipynb
    
    https://data.cdc.gov/Case-Surveillance/United-States-COVID-19-Cases-and-Deaths-by-State-o/9mfq-cb36
    
    This code shows case counts by state and is saved in the notebook titled: COVID19_State_Data_API_Calls.ipynb
    
**Transportation Security Agency checkpoint travel numbers for 2020 and 2019:**
    https://www.tsa.gov/coronavirus/passenger-throughput
  
    This data was copied from the TSA website and pasted into an Excel document, then saved on the local machine as a .csv file.
    
    Users wishing to reproduce the analysis will need to copy the TSA data from the website also.  
    
    This step is described in the Overview section of the COVID19Travel_Create_DataFrames.ipynb notebook.

# Project files:

**COVID19_Travel_Project_Presentation.pptx**
    
    Presents the project questions and results in PowerPoint presentation format.
    
    Visualizations are included along with link to this repository.

**Executive_Summary.ipynb**

    Summarizes the purposes of the analysis
    
    Displays each visualization with a short recap of the observations.
    
    Suggests future analysis to continue to study.

**COVID19_API_Calls.ipynb**

    Contains the code for making the API call to collect the CDC COVID data.
    
    Then case report date is converted to date format.
    
    Then the COVID data is grouped by case report date, with a count for deaths and hospitalizations.
    
    Finally, the group data is exported to a .csv file.

**COVID19Travel_Create_DataFrames.ipynb**

    Contains the code for combining the CDC and TSA data into a single DataFrame.
    
    Both types of data were called in from .csv files saved on my local machine.
    
    Dates were converted from objects to date datatypes
    
    TSA traveler numbers were converted from objects to floats
    
    The COVID counts (# cases, #deaths, # hospitalizations per day) are integers.

**COVID19Travel_Visualizations.ipynb**

    Contains the code for creating the visualizations and analyzing the data.

    Data was called in from .csv files saved in the COVID19Travel_Create_DataFrames.ipynb notebook.
    
    First, date is converted into DataFrames that can be plotted.
    
    Then the data is plotted in answer to key questions, with observations noted.
