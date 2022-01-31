# DSWECalibrationTool
Created to calibrate the USGS Dynamic Surface Water Extent algorithm to  Sentinel-2 data. It uses Monte Carlo simulation to randomize thresholds within 20% of the USGS defaults, deciding upon the best set using the ratio of high-confidence pixels within ground truth (lakes). A higher ratio of high- confidence pixels within lakes is desirable. 
Ultimately depreciated since the method is a bit flawed. As it prioritizes high confidence values in lakes, it doesn't take into account the algorithm can just assign
high confidence to EVERYTHING and call it good. So land is being misclassified, but as long as lakes are correctly classified the algorithm finds no issue. 
