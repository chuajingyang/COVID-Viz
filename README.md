# COVID-19 (in United States) Visualisations

# About
As part of my final interview for a Data Analyst Internship position in Dyson, I was tasked to analyse two COVID-19 related datasets and present my findings during the interview.

I pre-processed the data using Pandas in Jupyter Notebook, followed by visualisation and analysis in Tableau. I also prepared a presentation deck in PowerPoint for the presentation. I will just be sharing the Tableau Workbooks and datasets in this repository.

Ultimately, I did get the internship position but I had to reject it due to other reasons.

# Analysis

## Questions
Why does the number of confirmed cases vary so wildly between states in the US?
- Differences in adoption rate of preventive measures between states?
- What about demographic factors between states?

## Hypothesis
- Cause: The poorer the rate of adoption of preventive measures and/or the more susceptible the demographic groups of a state
- Effect: The higher the number of confirmed cases per capita for the state

## Features
### Preventive measures (Binary)
1. Worn a face mask
2. Avoided some or all restaurants
3. Cancelled or postpone pleasure, social or recreational activities
4. Avoided public or crowded places
5. Avoided contact with high risk people
6. Washed or sanitized hands

### Demographics (Multiple categories)
1. Age group
2. Household size
3. Region population density

## Pre-processing
I chose the 10 states in the dataset. I one-hot encoded the demographics columns, as the dataset will have to be multiplied by the relevant weights (recorded in the dataset as well). I then group the rows according to the states and aggregate the values of the features.

## Visualisation
I have 4 Tableau dashboards. Each of these dashboards is designed to compare the differences between the features of each state, and their corresponding differences of confirmed cases/100000.

The first dashboard is comparing the preventive measures between states, and how it affects the confirmed cases/100000. The next 3 dashboard is to compare the respective 3 demographic features between states, and how it affects the confirmed cases/100000.

## Evaluation
It is explained in greater detail in my presentation slides, but generally, only the last dashboard supports the hypothesis. There could be many reasons why the hypothesis is not supported (insufficient andpoor measures, etc.).

# Prerequisites
Tableau

# Author
Chua Jing Yang
