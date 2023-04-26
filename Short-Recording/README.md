# Analyze short photometry recordings

The code in this directory is designed for analyzing trials of up to a few hours in duration.

First, to analyze a single trial, use "Single_Trial_Analysis.ipynb". This script will analyze and save data from a single photometry trial (up to a few hours) combined with timestamps of events annotated from simultaneously acquired video or annotated in "real time". More information on data formats can be found within the script. The output of this script is a .pkl file with the processed data, as well as several graphs providing insight into the data.

Then, to group together multiple trials and analyze the combined data, use "Merge_Trials_and_Analyze.ipynb". The output of this script is a .pkl file with the combined data, and a number of graphs providing further insight.
