# DataScienceIndividualProject
Intro to Data Science Individual Project 

This dataset comes from testing done for an Advanced Wireless project. The data consists of the output from individual transmissions made using the acoustic data transmission application Wave-GUI (a side project made by Georgian coder Georgi Gerganov). Wave-GUI has 13 different protocols with which it can encode data. The original project’s goal was to find which of these protocols was the best carrier of data across a small variety of acoustic environments. 
In total, 975 discrete data transmissions were made, 195 per trial set. This data was analyzed by hand originally due to the author’s unfamiliarity with Python. 

In order to use the gathered data for this project, the spreadsheet needed to be cleaned up. All excel formulas used in the original project were deleted, and the sheets for each experimental trial set were deleted as well. This was done because these sheets contained repeated data so that it was easier to analyze within excel. The last step for data cleanup was to transpose the data so that the trial name was on top of the csv instead of the side. 

This project’s goal is to create a program that will be able to measure the metrics by which the data was analyzed automatically. It will be fed individual csv files, one for each protocol, and will measure each of the datasets using the following criteria: “% Some Output”, “% No Output”, “% Perfect Output”, “% Imperfect Output”, “% Single Frame”, and “% Multiple Frames”. The “% Some Output” and “% No Output” criteria denote the percent of trials that did or did not have any output. The “% Perfect Output” criterion denotes the percent of trials where the output was the exact smae as the input. The “% Imperfect Output” criterion denotes the perfect of trials where the output was not the exact same as the input. Finally, the “% Single Frame” and “% Multiple Frames” criteria denote the percent of trials where the output consisted of a single frame and the percent that consisted of multiple frames, respectively. “Frames” in this context refer to the number of lines of data interpreted by the Wave-GUI application for any given data transmission (ideally each trial would consist of a single frame of data). 

This project is useful because it would cut down on the time and effort needed to analyze the data created through the use of Wave-GUI. Unfortunately, the data must still be recorded by hand, as Wave-GUI does not have a way to export data.

A copy of the paper this data comes from is included in the Github repository.
