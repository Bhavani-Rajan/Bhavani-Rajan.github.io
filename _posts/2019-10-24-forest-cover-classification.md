---
layout: post
title: Forest Cover Classification
subtitle: 
bigimg: /img/forestcover_title.jpg
gh-repo: daattali/beautiful-jekyll
gh-badge: 
tags: [forest cover]
comments: true
---
## Goal
  Predicting forest cover type from cartographic variables only
	(no remotely sensed data).

## The Data
  The actual forest cover type for a given observation (30 x 30 meter cell) 
  was determined from US Forest Service (USFS) Region 2 Resource Information System 
(RIS) data.  Independent variables were derived from data originally obtained from 
  US Geological Survey (USGS) and USFS data.  Data is in raw form (not scaled) and contains
binary (0 or 1) columns of data for qualitative independent variables (wilderness areas and soil types).
  
  The study area included four wilderness areas found in 
	the Roosevelt National Forest of northern Colorado.  A total 
	of twelve cartographic measures were utilized as independent 
	variables in the predictive models, while seven major forest 
	cover types were used as dependent variables.  Several subsets 
	of these variables were examined to determine the best overall 
	predictive model. 
	
## Feature information
  
  * Elevation in meters
  
  * Aspect in degrees azimuth
  
  * Slope in degrees
  
  * Horizontal distance to nearest surface water features
  
  * Vertical distance to nearest surface water features
  
  * Horizontal distance to nearest roadway
  
  * Horizontal distance to nearest wildfire ignition points
  
  * Hillshade index at 9am, summer solstice
  
  * Hillshade index at noon, summer solstice
  
  * Hillshade index at 3pm, summer solstice
  
  * Wilderness area designation (4 binary columns)
  
  * Soil Type designation (40 binary columns)

## Target information
  
  * Forest Cover Type designation
  
## Data Cleaning and Feature Engineering
  Our Data is recorded observation with no null values.
  Two features( Wilderness area and Soil type),which are the binary columns, spanning 44 columns instead of two.
  Bringing the 44 columns down to 2 columns made model perform better. 

## Baseline prediction
 Simply predicting the most frequently found tree gives under 50%. we need to engineer a model that beats the baseline accuracy

**Types of trees that cover the forest**

![Types of trees that cover the forest](/img/forest cover.png)

**Distribution of trees that cover the forest**

![Distribution of trees that cover the forest](/img/Forest cover dist.png)

## Data Exploration

**Forest Cover Vs Elevation, Aspect, Slope **

![Forest Cover Vs Elevation, Aspect, Slope](/img/fc_ele_as_sl.png)

**Forest Cover Vs Horz Dist from water features, Vert Dist from water features, Horz Dist to roadways, Horz Dist to wildfire ignition pts  **

![Forest Cover Vs distances](/img/fc_dist.png)

**HillShade at 9 am , Noon, 3 pm Vs Forest Cover**

![Forest Cover Vs hillshade](/img/fc_hs.png)


## Selection of the model

## Feature importances

## Summary

The map clearly shows the rise of this disease in south eastern and few regions of eastern United States compared to the other parts of United States. 
