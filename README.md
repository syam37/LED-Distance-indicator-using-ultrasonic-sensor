# LED-Distance-indicator-using-ultrasonic-sensor
The project is designed to develop distance measurement system using ultrasonic waves and interfaced with arduino. We know that human audible range is 20hz to 20khz. The distance of an obstacle from the sensor is measured through ultrasonic sensor. After knowing the speed of sound the distance can be calculated.


**COMPONENTS:**

●	Arduino Uno
●	Ultrasonic sensor (HC-SR04)
●	LED Different colours
●	Scale
●	Bread board
●	Power supply
●	Jumper  wires
●	Resistors 220 ohms

**CIRCUIT DIAGRAM:**
![image](https://github.com/syam37/LED-Distance-indicator-using-ultrasonic-sensor/assets/66241030/536db242-fa0f-4761-9342-cd07ed82d714)




**WORKING:**                                                                                                              
You will write a program that is constantly reading information from the ultrasonic sensor. According to the distance measured by the sensor the red or the green LED will turn on.
For this to happen you will use the next condition: If the distance is less than 20 cm, the red LED will be on and the green LED will be off; but if the distance is more than 20 cm, the green LED will be on and the red LED will be off.
To measure the distance you have to define TRIG Pin as an output and ECHO as an input. TRIG will send the ultrasonic waves forward and ECHO will be waiting for the waves to come back.
Then, each time a wave comes back, you have to measure the distance of the object. Remember that the speed of sound in the air is always: 343,2 m/s.
So if you know the total time of the wave to go and come back you will have to calculate the distance. For that, you have to divide by 2 the total time the wave goes and comes back and then you multiply it by the speed of sound in the air:
Distance = 343m/s *time (seconds)
To work with a better resolution, you will work with cm/us (centimeters / microseconds) using the next conversion:
Once you have calculated the distance you will need to turn the red or the green light. For that to happen, you have to determine as output both pins where you have the connected the two LEDs. And when you want to turn on one of them you have to give it a HIGH value ( 1) and when you want it to be off you have to give it a LOW value (0).                                                                                                    

