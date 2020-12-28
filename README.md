# Predicting criticality of an aircraft fault by its description
## Project Description

An MEL C is intended to permit operation with inoperative instruments or equipment for a period of time until repairs can be accomplished - it is not a "free pass." Repairs must be accomplished at the earliest opportunity.
In the following project we will be analyzing the categorie MEL C, which has the time limit of 10 days after its opening to be executed. The main question is if it's possible to predict the criticality of a fault by its description. A MEL C can be opened by the pilot/crew during a flight or the mechanic during an inspection, they write the description of each fault and this information remains vinculated to each "barcode".

## Files
1. Aircraft-Faults-Description.ipynb: contains the analysis, visualization, modeling and results of the data.
2. A320_dataset.csv: contains the dataset, to model and analysis on faults.

## Results
In this project I analyzed and built a classifier model that predicted the criticality of aircrafts faults. The work began with some data cleaning, removing all the data that was unnecessary to our goal. Answering some business questions that can provide some insights to how the fleet behaved in the last years. And then the data preparation for the machine learning model. Dividing the data between normal, risk and aog faults to try to provide a prediction whether future tasks will generate risk to the operation. These fault's descriptions didn´t provide much information about "risk" and "aog" criticality, where we could only predict around 15% in these categories. But in general it´s was possible to achieve a 76% of accuracy in this model. With the suggested improvements, in the model and in the process of inputting a description, it's possible to obtain a higher number of accuracy for each category. Overall when these models get to production and decisions start to be made by these results, the gain in avoiding delays and cancelled flights can be huge for the company.nd where the biggest problem lays and initiate changes in those processes to get a better solution on open faults.

For more information about the results an article has been written on this project <a href="https://gabrielpeixoto-5587.medium.com/predicting-criticality-of-an-aircraft-fault-by-its-description-66e95b6eb7e4">here</a>.

## Requirements
Anaconda, pandas, numpy, matplotlib, seaborn, Scikit learn and StringIO

## Licensing, Authors, Acknowledgements
* LATAM Airlines for providing the dataset respecting the rules of data confiability of the company.
* Stackoverflow for helping with some coding.
* Udacity Data Science Nanodegree for providing the knowledge and tools for this challenge.
