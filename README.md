# Solar Plant Forecaster

Final project for the Building AI course

## Summary

The idea with the project is to create a tool too forecast energy production from a solar plant to know coming available energy and need of external energy inflow. This enables a way to control usage and storage of energy to control the buying and selling of electric energy.

This will be a base for energy planning knowing what energy to add, store and consume.

Using historical energy production combined with historical weather and schedule of sunrise and set, the system will be trained to predict coming energy production based on weather forecast.

## Background
Electric energy produced from solar plant is varying with incoming radiation, which is based on the weather conditions. This makes the need of external, incoming, electricity supply varying. 

Having a tool to predict energy production, makes it possible not only to plan energy consumption but also storage of energy. Storage could be done using the heated water (boiler), electric car or a an external battery.

This would benefit sustainability by lowing the external electric grid load. Besides environmental benefits, the cost of grid charge and less bought energy, there is an educational purpose.

## Data and AI techniques
The data needed to set up and train the tool are 
- Historical energy production Used for training the tool and verification of how the tool performs

- Historical local weather Used for training the tool. The weather highly impacts on radiation, i.e. light, reaching the solar cells.
Schedule for sunrise and sunset Whether it is an advantageous weather or not, with direct light or not, it is only when sun is up that there will be energy production.

- Weather forecast The base for predicting energy production

Future improvement could be to measuring the temperature of the solar cells. Both as input to the model and a parameter to predict.

A neural network will be trained to predict future energy production.

The hourly sample rate will be used.

## How is it used
The tool will be used for a private solar plant for home purpose.

## Challenges
Ones energy production is predicted, the control of energy external inflow, usage or storage is not solved by the tool.

Feeding historical data to the tool is manually done.

## What next
The following improvements could be done further on
Trim the prediction model As insight and experiences are made, there will be a continuous work to improve and trim the prediction model.
Automated feed of historical data Automation of feeding historical weather and energy production data.
Interface to energy dispatcher Predicted energy production should be forwarded to decision making of energy usage and trading, i.e storage, buy or sell of energy. 

## Acknowledgments
This is a work triggered by the course Building AI by Reaktor, University of Helsinki. Models, code etc will probably be based on the examples from the course.
