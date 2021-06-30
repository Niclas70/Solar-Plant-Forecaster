# Solar Plant Forecaster - Implementation
In this implementation, machine learning was used to forecast energy production based on weather prognosis and sun angle parameters.

This is the final thesis work of the course Building AI.  

## Input parameters

- Azimuth. Compass direction of the sun.
- Altitude. Angle height of the sun.
- Temperature. Air temperature in Celsius.
- Rain. Rain in mm.
- Clouds. Cloud in percent.
- Wind. Wind in m/s.

The sun angles were given by tables based on location, date and time. The other parameters were downloaded from the Swedish meteorological institute, SMHI, from the closest weather station about 13 km to the east of the plant.

## Output parameter
Output electrical energy was extracted from en solar converter.

## Training data
The parameters were picked from the f 1st say in the month's Mars to October, i.e. 10 days. For each day hourly samples were made from sunrise to sunset.

In total 114 values of training data.

## Test data
The parameters were picked from the 15th day in the month's Mars to October, i.e. 10 days. For 08.00, 12:00 and 16:00 o'clock. each day hourly samples were made from sunrise to sunset.

In total 24 values of test data.

## Model
As a model, a sequential TensorFlow model was used
- The Input layer is normalized.
- The second layer of 100 nodes activated by ReLU.
- The third layer of 80 nodes activated by Linear.
- The output layer of 1 node activated by Linear.

Epoch was set to 2000.

## Result
The loss in fitting the training data was 0.04 
The loss of the test data was 14.68

![GitHub Logo](/DiagramSolarPlantForecast.png)

Blue: True value. Test output. 
Orange: Predicted value. Model output.

## Summary
The model parameters could certainly be better fitted by further elaboration.
The distance to the weather station, 13 km, gives an uncertainty of local weather, which could be delayed, earlier, or inaccurate.
There is a strong correlation between sun angles and temperature, i.e. season and time of the day.
There’s a rather strong correlation between sun angles and weather parameters in generated electrical energy from a solar plant.

## Next step ##
The next step is to implement calculation of forecast of coming days total energy production, based on weather prognosis and compare to true energy output.
