# Fuzzy Tip Recommender using skfuzzy

This project implements a fuzzy logic system to recommend tips based on six input attributes: Food Quality and Service Quality, each represented as multi-dimensional vectors. 

## Input Attributes
- **Food Quality**: 
  - Food Temperature
  - Food Flavor
  - Portion Size
- **Service Quality**: 
  - Attentiveness
  - Friendliness
  - Speed of Service

## Functionality
The user can input values for the six measures and receive a recommended tip as a percentage of the final bill. The program prompts the user to enter another set of measures until the user chooses to exit. Inputs are validated to ensure they are within the acceptable range and legal values for each attribute.

## Implementation
- Utilizes skfuzzy to create a fuzzy tree for tip recommendation.
- Defines a data structure in Python to hold control objects for each FIS.
- Passes outputs of the Food Quality and Service Quality FISs as inputs to the Tipper during control simulation.
- Implements rules for each FIS and determines the number of and parameters for fuzzy sets in each input dimension.
- Employs center-of-gravity defuzzification in all three FIS for accurate tip recommendation.

