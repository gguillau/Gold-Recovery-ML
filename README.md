# Gold-Recovery-ML
Real data science problem from the gold mining sector. This project is provided by Zyfra.

## Background

This project is part of the Data Scientist training program from Practicum by Yandex. More info in link below:

https://practicum.yandex.com/data-scientist


## Objective

Prepare a prototype of a machine learning model for Zyfra. The company develops efficiency solutions for heavy industry. The model should predict the amount of gold recovered from gold ore. You have the data on extraction and purification. The model will help to optimize the production and eliminate unprofitable parameters. You need to:

- Prepare the data;
- Perform data analysis;
- Develop and train a model.

### Technological Process
How is gold extracted from ore? Let's look into the process stages. Mined ore undergoes primary processing to get the ore mixture or rougher feed, which is the raw material for flotation (also known as the rougher process). After flotation, the material is sent to two-stage purification.


Process Details:

- Flotation Gold ore mixture is fed into the float banks to obtain rougher Au concentrate and rougher tails (product residues with a low concentration of valuable metals). The stability of this process is affected by the volatile and non-optimal physicochemical state of the flotation pulp (a mixture of solid particles and liquid).
- Purification The rougher concentrate undergoes two stages of purification. After purification, we have the final concentrate and new tails.

## Data description

### Technological process
 * Rougher feed — raw material
 * Rougher additions (or reagent additions) — flotation reagents: Xanthate, Sulphate, Depressant
 * Xanthate — promoter or flotation activator;
 * Sulphate — sodium sulphide for this particular process;
 * Depressant — sodium silicate.
 * Rougher process — flotation
 * Rougher tails — product residues
 * Float banks — flotation unit
 * Cleaner process — purification
 * Rougher Au — rougher gold concentrate
 * Final Au — final gold concentrate

 Parameters of stages
* air amount — volume of air
* fluid levels
* feed size — feed particle size
* feed rate

### Feature naming
 Here's how you name the features:
* [stage].[parameter_type].[parameter_name]
* Example: rougher.input.feed_ag
*** Possible values for [stage]:**
* rougher — flotation
* primary_cleaner — primary purification
* secondary_cleaner — secondary purification
* final — final characteristics

*** Possible values for [parameter_type]:**
* input — raw material parameters
* output — product parameters
* state — parameters characterizing the current state of the stage
* calculation — calculation characteristics

##  Libraries Used
 * Pandas
 * Matplotlib.pyplot
 * scipy.stats
 * numpy
 * sklearn

##  Models Evaluated
 * LinearRegression
 * RandomForestRegressor
 * DecisionTreeRegressor
