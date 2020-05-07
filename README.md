# This is CS50x Final Project
This system used to detect anomaly obtained in the temperature in the freezer and send an alert via message &amp; tweet.

Present time Technologies are much important in each and every person's life. There are lots of digital technologies in the technical market. I choose Internet Of Things and Machine Learning powered by Bolt IoT for this project. This project Freezer Monitor & Anomaly System can be helpful where IoT is used to take the temperature reading from the temperature sensor as input and Machine Learning is used to find the anomaly of the temperature using the Z-Score analysis. Anomaly means differ from normal state. In this system when a anomaly in the temperature is detected, LED is start glowing and Buzzer start buzzing for 2 seconds and turn off and immediately an alert will be sent to the mobile as SMS and Twitter Tweet as well.

This system is used in the industrial big freezers where temperature has to be maintained within boundaries.


Hardware Requirement:

Bolt IoT Wi Fi Module
LM35 Temperature Sensor
Buzzer
Male to Female jumperwires
USB cable

CONNECTIONS:

Connect Bolt IoT WiFi Module to some power supply using the USB cable
connect LM35 temperture sensor to the Bolt WiFi Module
VCC pin of the LM-35 Sensor is connected to 5 V. of the Bolt WiFi Module.
Output pin of the LM-35 is connected to A0 (Analog input pin) of the Bolt WiFi Module
GND pin of the LM-35 is connected to the GND
Connect Buzzer and LED to the Module
Negative PINs of both elements connects to the GND and Positive PINs connects to GPIO Digital PIN '1'

 Algorithm:

Step-1: Fetch the latest sensor value from the Bolt device.

Step-2: Store the sensor value in a list, that will be used for computing Z-Score.

Step-3: Compute the Z-Score and upper and lower threshold bounds for normal and anomalous readings.

Step-4: Check if the sensor reading is within the range for normal readings.

Step-5:If it is not in range, send the SMS and tweet as well

Step-6: Wait for 10 seconds.

Step-7: Repeat from step 1.

Z-SCORE ANALYSIS:

Z-score analysis is used for anomaly detection. Anomaly here means a variable's value (light intensity of the surroundings) going beyond a certain range of values. The range of values is called bounds (upper bound and lower bound). These bounds are calculated using the input values, frame size and multiplication factor. The frame size is the minimum number of input values needed for Z-score analysis and the multiplication factor determines the closeness of the bounds to the input values curve.



