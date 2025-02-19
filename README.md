# Time Series Project - [Acea Smart Water Analytics Challenge in Kaggle](https://www.kaggle.com/competitions/acea-water-prediction/data)


The goal of this project is to predict for Acea Group (one of the leading Italian multiutility operators in the water services sector supplying 9 million inhabitants), the most efficient water availability, in terms of level and water flow for each day of the year, in order to help preserve the health of the waterbodies in the areas o Lazio, Tuscany, Umbria, Molise, Campania (Italy).

## Data structure

This analytics competition uses datasets that are completely independent from each other. However, it is critical to understand total availability in order to preserve water across the country.

Each dataset represents a different kind of waterbody. As each waterbody is different from the other, the related features are also different

The Acea Group deals with four different type of waterbodies: water springs, lakes, rivers and aquifers.

The Acea Group deals with four different type of waterbodies: 
* water spring (for which three datasets are provided)
* lake (for which a dataset is provided)
* river (for which a dataset is provided)
* and aquifers (for which four datasets are provided).


## Challenge

To predict the amount of water in each unique waterbody

To determine how features influence the water availability of each presented waterbody

# Intervals
Models should capture volumes for the specific time interval (day/month) of each waterbody (for instance, for a model working on a monthly interval a forecast over the month is expected).

# Expected Outcome

A notebook that can generate 4 mathematical models, one for each category of waterbody (acquifers, water springs, river, lake) that might be applicable to each single waterbody.


1. **Waterbody: Auser (Type: Aquifer)**
Two subsystems: 
    * NORTH: The former partly influences the behavior of the latter. The levels of the NORTH sector are represented by the values of the SAL, PAG, CoS and DIEC wells.
    * SOUTH: The levels of the SOUTH sector are represented by the LT2 well. 
 

2. **Waterbody: Petrignano (Type: Aquifer)
The groundwater levels are influenced by the following parameters: rainfall, depth to groundwater, temperatures and drainage volumes, level of the Chiascio river.

3. **Waterbody: Doganella (Type: Aquifer)
The aquifer levels are influenced by the following parameters: rainfall, humidity, subsoil, temperatures and drainage volumes.

4. **Waterbody: Luco (Type: Aquifer)
Accessed through wells called Well 1, Well 3 and Well 4 and is influenced by the following parameters: rainfall, depth to groundwater, temperature and drainage volumes.

5. **Waterbody: Amiata (Type: Water spring)**
Accessed through Ermicciolo, Arbure, Bugnano and Galleria Alta water springs. 
The levels and volumes of the four sources are influenced by the parameters: rainfall, depth to groundwater, hydrometry, temperatures and drainage volumes.

6. **Waterbody: Madonna di Canneto (Type: Water spring)
Supplied by the water catchment area of the river Melfa.

7. **Waterbody: Lupa (Type: Water spring)

8. **Waterbody: Arno (Type: River)**
The availability of water for this waterbody is evaluated by checking the hydrometric level of the river at the section of Nave di Rosano.

9. **Waterbody: Bilancino (Type: Lake)**
Artificial lake, during the winter months, the lake is filled up and then, during the summer months, the water of the lake is poured into the Arno river.

# Important consideration on the correlation between features and date
It is of the utmost importance to notice that some features like rainfall and temperature, which are present in each dataset, don’t go alongside the date. 
**Indeed, both rainfall and temperature affect features like level, flow, depth to groundwater and hydrometry some time after it fell down.**
This means, for instance, that rain fell on 1st January doesn’t affect the mentioned features right the same day but some time later. As we don’t know how many days/weeks/months later rainfall affects these features, this is another aspect to keep into consideration when analyzing the dataset.

