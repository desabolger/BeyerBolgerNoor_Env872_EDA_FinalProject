---
output: bookdown::pdf_document2

---
# BeyerBolgerNoor_Env872_EDA_FinalProject

## Summary

This dataset was created for the Final Course Project for Environmental Data Analytics (ENV 872L) at Duke University, Fall 2023. 

This dataset contains data from a study titled “Seagrass growth rates and physical characteristics and measures of water temperature and salinity during a simulated green turtle grazing experiment in The Bahamas, 1999 – 2000,” done in 2022 by Johnson, Hanes, and Bolten. Data was collected to explore abiotic factors controlling seagrass growth and the effects of simulated green turtle grazing. 

## Investigators

Repository Creators:

Emma Beyer
Nicholas School of the Environment, Duke University
emma.beyer@duke.edu

Desa Bolger
Nicholas School of the Environment, Duke University
desa.bolger@duke.edu

Nusrat Noor
Nicholas School of the Environment, Duke University
nusrat.noor@duke.edu

Principal Researchers of study:

Dr.  Robert Johnson
University of Wisconsin-Madison
robert.a.johnson@wisc.edu
0000-0003-4072-5623
        
        
Dr.  Kathleen Hanes
Washington University in St. Louis
khanes@wustl.edu
        
        
Dr. Alan Bolten
University of Florida
abolten@ufl.edu
0000-0002-4834-2742
        
        
Dr. Karen Bjorndal
University of Florida
bjorndal@ufl.edu
0000-0002-6286-1901


## Keywords

Seagrass, Bahamas, Green Turtles, Salinity, Temperature, Linear growth, Production Rates

## Database Information

Data were collected from a study on seagrass (Thalassia testudinum) in Lee Stocking Island, Exumas, The Bahamas.  More information can be found here: https://portal.edirepository.org/nis/mapbrowse?packageid=edi.422.1

Data were collected using the Data tool (EDI Data Portal). 

csv files were saved as 'Temperature-Salinity.csv', 'Seagrass-structure.csv', 'Seagrass-production-rates.csv', 'Segrass-linear-growth-rates.csv', and 'Seagrass-aboveground-biomass.csv'. 

Data were accessed 2023-11-01. 

## Folder structure, file formats, and naming conventions 

Within the 'BeyerBolgerNoor_Env872_EDA_FinalProject' file you will find the 'Output', 'Data', and 'Code' files. 

In the 'Output' file, you will find the final Rmarkdown report on our findings. This will be a single Rmarkdown file. 

In the 'Data' file, you will find the data used within this analysis. Raw data was placed within the 'Raw' folder, processed data was placed in the 'Processed' file, and the metadata information was placed in the 'Metadata' file. Both the 'Raw' and 'Processed' files are in csv formats. The 'Metadata' files are in txt formats.

In the 'Code' file, you will find all the rmarkdown files and PDFs associated with the analysis of the data. This analysis was done in Rmarkdown files and then knit into PDF versions for reader accessability. Each Rmarkdown was named according to the analysis that was preformed. 

## Metadata

File: Temperature-Salinity.csv

Column Name | Description | Class of Data | Units 
:------------| :----------------------| :--------------| :------------
treatment  | grazing treatment of "reference", "summer", or "winter". | chr | no units
date | date when the measurements were taken | chr | YYYY-MM-DD
exp_week | experimental week ID assigned throughout the experiment | int | no units
min_temp | minimum temperature taken on that day | num | degrees C
max_temp | maximum temperature taken on that day | num | degrees C
salinity | water salinity reading at each location | num | g/kg

File: Seagrass-structure.csv

Column Name | Description | Class of Data | Units 
:-------------|:----------------------------|:---------------|:---------------
plot | number ID associated with each plot site | int | no units 
treatment | grazing treatment of "reference", "summer", or "winter". | chr | no units 
date | date when the measurements were taken | chr | YYYY-MM-DD 
interval | number of times the variable has been measured | int | no units 
exp_week | experimental week ID assigned throughout the experiment | int | no units 
blade_length | seagrass blade length  | num | cm 
blade_width | seagrass blade width  | num | cm 
shoot_density | seagrass shoot density  | num | number per meter squared 
bps | number of seagrass blades per shoot  | num | no units 
lai | leaf area index  | num | meter squared per meter squared 

File: Seagrass-production-rates.csv

 Column Name | Description | Class of Data | Units 
:-------------|:------------------|:---------------|:---------------
plot | number ID associated with each plot site | int | no units 
treatment | grazing treatment of "reference", "summer", or "winter". | chr | no units 
date | date when the measurements were taken | chr | YYYY-MM-DD 
interval | number of times the variable has been measured | int | no units 
exp_week | experimental week ID assigned throughout the experiment | int | no units 
gr_mass | rate of seagrass mass growth (i.e., production), as dry mass | num | gram per meter squared per day 

File: Seagrass-linear-growth-rates.csv

 Column Name | Description | Class of Data | Units 
:-------------|:--------------------|:---------------|:--------------
plot | number ID associated with each plot site | int | no units 
treatment | grazing treatment of "reference", "summer", or "winter". | chr | no units 
date | date when the measurements were taken | chr | YYYY-MM-DD 
interval | number of times the variable has been measured | int | no units 
exp_week | experimental week ID assigned throughout the experiment | int | no units 
gr_length | linear growth of seagrass | num | cm 

File: Seagrass-aboveground-biomass.csv

 Column Name | Description | Class of Data | Units |
:-------------|:--------------------|:---------------|:-------------
plot | number ID associated with each plot site | int | no units 
treatment | grazing treatment of "reference", "summer", or "winter". | chr | no units 
date | date when the measurements were taken | chr | YYYY-MM-DD 
interval | number of times the variable has been measured | int | no units 
exp_week | experimental week ID assigned throughout the experiment | int | no units 
ag_biomass | above ground seagrass biomass, as dry mass | num | gram per meter squared 

## Scripts and code

File: temp_lineargrowth.Rmd
Rmarkdown containing the analysis of temperature and salinity on seagrass linear growth.

File: temp_lineargrowth.pdf
PDF of the Rmarkdown of the same name.

File: Seagrass_vs_Production_Rates.Rmd
Rmarkdown containing the analysis of seagrass production rates and temperature.

File: Seagrass_vs_Production_Rates.pdf
PDF of the Rmarkdown of the same name.

File: Salinity_vs_Production_Rates.Rmd
Rmarkdown containing the analysis of seagrass production rates and salinity.

File: Salinity_vs_Production_Rates.pdf
PDF of the Rmarkdown of the same name.

File: Final_Project.Rmd
Rmarkdown containing all the graphs and analysis.

File: Final_Project.pdf
PDF of the Rmarkdown of the same name.



