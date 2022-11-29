# Project: **ML Model Predicting the Recovery of Gold**

## Description and Purpose of Project:
Zyfra, a company that develops efficiency solutions for heavy industry, needed a  prototype of a machine learning model to predict the amount of gold recovered from gold ore. They provided with data for extraction and purification stages of gold recovery. To build the machine learning model, Zyfra provided us with following documentations about the different processes that occur during the recovery of gold: 
- Mined ore undergoes primary processing to get the ore mixture or rougher feed, which is the raw material for flotation (also known as the rougher process). After flotation, the material is sent to two-stage purification.
1. Flotation: Gold ore mixture is fed into the float banks to obtain rougher Au (gold) concentrate and rougher tails (product residues with a low concentration of valuable metals).
The stability of this process is affected by the volatile and non-optimal physicochemical state of the flotation pulp (a mixture of solid particles and liquid).
2. Purification: the rougher concentrate undergoes two stages of purification. After purification, we have the final concentrate and new tails.

The process can be explained in the image below:

<img src="Image (1).png" height = 400>

For the calculation of gold recovery, we used the following formula: 
<img src="Image (2).png" height = 200>

where:

- C — share of gold in the concentrate right after flotation (for finding the rougher concentrate recovery)/after purification (for finding the final concentrate recovery)
- F — share of gold in the feed before flotation (for finding the rougher concentrate recovery)/in the concentrate right after flotation (for finding the final concentrate recovery)
- T — share of gold in the rougher tails right after flotation (for finding the rougher concentrate recovery)/after purification (for finding the final concentrate recovery)

For the evaluation metric, we used sMAPE, symmetric Mean Absolute Percentage Error dpicted below: 
<img src="Image (3).png" height = 200>

The denotation of sMAPE are the following:

<img src="Image (4).png" height = 100>
Value of target for the observation with the i index in the sample used to measure quality. 

<img src="Image (5).png" height = 100>
Value of prediction for the observation with the i index, for example, in the test sample.

<img src="Image (6).png" height = 100>
Number of observations in the sample.

<img src="Image (7).png" height = 100>
Summation over all observations of the sample (i takes values from 1 to N).

Using the models, we need to predict two values:
- rougher concentrate recovery rougher.output.recovery
- final concentrate recovery final.output.recovery

The values will be go into the final metric, which includes these two values:

<img src="Image (7).png" height = 200>
## Business value:

## Tools and concepts used in project:

## Table of contents:

