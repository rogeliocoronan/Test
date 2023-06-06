# Test
Tests
June 6th, 2023
*****************************************************
The current analysis and results were written in R version 4.2.2
To reproduce the results it is necessy use the library(raster)
The country boundaries come from ESRI (https://hub.arcgis.com/datasets/esri::world-countries-generalized/about)


*****************************************************
To reproduce the results all necessary steps are included in the script


To fully reproduce the excersice it is necessary to:
(1) ammend the next directory path (path.IIASA) where all the data is included
(2) Download from ESRI the country boundaries
(3) Adjust the Original names reported in the NUE data.set (Zhang_et_al_2015). I adjusted the names to align with the names in the Country shapefile
(4) It is necessary to create 3 sub-folders with in the path "path.IIASA":
00_Data
02_Figures
03_Data_export


*****************************************************
Answer to questions 4, 5 and 6.
4.
Globally, wheat production and nitrogen surplus show a strong positive trend (p<0.001), but there is no relationship between wheat production and 
nitrogen-use efficiency (NUE) (p>0.2). However, among the top-10 wheat producers, there is a significant inverse association between nitrogen losses 
and NUE (p<0.008), contrasting the global pattern (p>0.1).

5. 
In FLAM, it would be beneficial to incorporate nitrogen deposition following shifting cultivation as a means to assess the N-return to the system. 
However, a potential limitation lies in the spatial resolution of nitrogen-use efficiency (NUE) compared to the sizes of shifting cultivation parcels.
 As for GLOBIOM, I believe that by modeling land-use trajectories, it becomes feasible to evaluate the nitrogen cycle.

6. 
a) Initially, I encountered difficulties uploading the original shapefile (g2015_2005_2.shp) containing country boundaries, as it was quite large (700 Mb). 
Consequently, I opted for a more generalized version of global country boundaries, significantly reducing the file size to 3.3 Mb. This adjustment notably 
improved processing time.
b) The country names in the NUE csv file did not completely align with the names in the Country shapefile. To address this, I created a modified version of the 
NUE dataset, ensuring that the names corresponded accurately with my dataset
