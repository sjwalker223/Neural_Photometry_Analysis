# Analyze long photometry recordings

The code in this directory is designed for analyzing trials of multiple hours to days in duration. In addition, it can optionally incorporate simultaneously acquired behavioral data from a "FED3" device, which measures food-seeking and -retrieval behaviors.

First, to analyze a single trial, use "Single_Overnight_Analysis.ipynb". This script will analyze and save data from a single photometry trial (up to a few hours) combined with timestamps of specific events. More information on data formats can be found within the script. The output of this script is a .pkl file with the processed data, as well as several graphs providing insight into the data.

Second, if FED3 data was acquired, use "Single_Overnight_FEd3.ipynb". This script will analyze the FED3 data, align it to the photometry recording, and save the combined data. The output of this script is a .pkl file with the combined photometry/FED3 data from this trial, in addition to a number of graphs describing the data.

Then, if FED3 data **was not** acquired: to group together multiple trials and analyze the combined data, use "Merge_Overnight_Trials_and_Analyze.ipynb". The output of this script is a .pkl file with the combined data, and a number of graphs providing further insight.

Alternatively, if FED3 data **was** acquired: to group together multiple trials and analyze the combined data, use "Merge_Overnight_Trials_and_Analyze-with_FED3.ipynb". The output is a .pkl file with the combined FED3/photometry data from multiple trials, and numerous graphs representing behavior and neural activity.
