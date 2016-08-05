# ENVI ROI Processing

This project has code that will process and format output from ENVI's ROI spectral libraries

### Dependencies
#### For Extracting_ROI.py:
Requires numpy library

---
### Code Descriptions:
#### For Extracting_ROI.py:
This code reads through a spectral library metdata file created with ENVI and formats it into .csv.
Each row of the csv is one item in the spectral library. Does not include RGB value of ROI.
Does include Name, # of Points, spectral information, and other information the user chooses to include in ENVI output
(such as X, Y, MapX, MapY, Lat, Lon).
This code takes two inputs:
1. The original spectral library from ENVI
2. Output file name
---
### Building spectral libraries:
Using ENVI, in the menu for your image select Tools > Region of Interest > ROI tool. A new dialog will open call ROI Tool.
Open your Regions Of Interest (ROIs) by selecting File > Restore ROIs. To extract the spectral information at the ROI locations, select 
File > Output ROIs to ASCII. In the next dialog, select the image that contains the spectral information you want to extract and hit next.
In the following, select which ROIs you would like to extract and choose an output filename. This is the output that the project is editing
and processing. 