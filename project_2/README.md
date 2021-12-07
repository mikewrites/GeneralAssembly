# Table of contents

## root
  * This document
  * Presentation
      * a slide deck accompaning my final pesentation.

## /code

  * BK_Changes
      * Most notebooks are extensively commented, and interspersed wth visualiztions that illustrate what I was doing and the thought process behind my choices. This notebook provides an organized, high-level view of my code. All code that changed something about the provided datasets, is reconstructed there. Its also designed to offer a way to skip ahaed to any notebook you want to run without relying on the instances of the .pkl files that have already been generated. Please use this if you don't want to run all notebooks in the specified order or something might break. 
      **Update I got a little carried away tweaking things and my Feature Engineering notebook is hopelessly disorganized. I'm going to leave my notes and the raw code there, but I prefer you run this file to generate your modeling sets.The other should work, but this one is more systematic and thus safer.**
  * 1_Cleaning.ipynb
      * Most of my preliminary data cleaning is documented in this notebook, of course data cleaning is an endless process and there were small changes which I might have made in other notebooks.
  * 2_EDA.ipynb
      * This notebook contains most of my exploratory data analysis, many of my visuals are also generated here. There's a lot of overlap between the EDA and Feature Engineering notebooks, including places where the reader is prompted to switch to the other book. Roughly, I've tried to discuss the resoning behind changes I made to features in this notbook, and talk about the technical details in the next.
  * 3_FeatureEngineering.ipynb
      * Roughly, an attempt to document the process of feature engineering, as opposed to discussion of why I made those changes. While it shoud be working code, it's now to document my process
  * 4_Modeling 
      * This notebook contains all models and most model evaluation. Model evaluation accompanied by charts and graphs is in the following notebook.
  * 5_Visualizations
      * Most visualization intended for my completed project are generated here. Visualaztions generated to help me understand my data are in the EDA folder. Where these two categories overlap, I try to include them in both notebooks.
  
## /datasets
   * provided materials:
       * sample_sub_reg.csv, test.csv, train.csv, rdme.md, suggestions.md are preserved as they were assigned. These describe the assignment to which this project is a response
   * /pickles
       * space for .pkl files, a format used to save and transfer dataframes between notebooks
   * /final
       * my final data and visualizations


# Business Question
  
This project was built aroung the following question: How can feature engineering reduce the dimensionality of data while maintaining the signal? It's oriented towards technically literate financial executives who are considering contracting with my data science firm. They have already gotten information about value added for past clients, but have asked me to give them a better idea of what a data scientist actually does. To illustrate my role, I walk them through my process in creating a linear regression model that incorporates a large amount of catagorical data without overfitting. I contrast this to two bad models: an underfit one created by considering only numeric features and an overfit one consisting of numeric data plus one hot encoding of all categorical features.

# Executive Summary

I first created two baseline models, one with the train.csv file's numeric data and the other with all non-numeric data encoded with one hot. Then I engaged in feature engineering to reduce the dimesionality of the data. though I was successful as substrantially reducing the dimensionality, in the end the baseline numeric model was the best predictor. I belive the issue is that there were a lot of numeric features and a high degree of redundancy between the signal in the numeric data and the signal in the categorical data. 


# Data Documentation

Given the large number of features in this dataset, and the exellent documentation available here, (http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)  I'm going to let the reader get it. My code is extensivelly documented.






```python

```
