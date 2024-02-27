# IOT-BASED-AUTOMATIC-FIRE-DETECTION-ALERT-SYSTEM-AND-EXTINGUISHER
<h2>ABSTRACT</h2>
<p >The rapid integration of Internet of Things (IoT) technologies has revolutionized various domains, including fire safety and emergency response systems. This projects proposes an IoT-based automatic fire detection, alert system, and extinguisher for enhanced fire prevention and management. The system employs a network of smart sensors strategically placed in sensitive areas to continuously monitor the environment for signs of fire.The sensor nodes are equipped with advanced fire detection algorithms that can quickly and accurately identify the presence of flames, smoke, or elevated temperatures. Upon detection, the system triggers an immediate alert through a secure communication channel, notifying relevant stakeholders such as building occupants, emergency services, and facility managers.In addition to the alert system, the proposed solution includes an integrated smart extinguisher mechanism. The IoT-based extinguisher is capable of autonomously navigating to the detected fire location using real-time data from the sensor network. The extinguisher utilizes artificial intelligence and machine learning algorithms to optimize its path and extinguishing technique based on the type and intensity of the fire. Furthermore, the system incorporates cloud-based analytics to provide comprehensive insights into fire patterns and trends, enabling proactive measures for future prevention. 
</p>
<h2>COMPONENTS</h2>
1.	ESP32 <br>
2.	FLAME SENSOR <br>
3.	GSM MODULE 900A <br>
4.	WATER PUMP MOTOR[EXTINGUISHER] <br>
5.	5V RELAY <br>
6.	BUZZER <br>
<h2>CIRCUIT DIAGRAM</h2>
<img src="https://github.com/Ajay12ks/IOT-BASED-AUTOMATIC-FIRE-DETECTION-ALERT-SYSTEM-AND-EXTINGUISHER/assets/138428990/f6510612-68a3-4c16-9b51-916c26843d4a"> <br>
<h2>HARDWARE SETUP</h2>
<P>
  
1.	Connect SIM800L to ESP32: <br>
•	Connect the Tx pin of the SIM800L module to digital pin 19 on the ESP32. <br>
•	Connect the Rx pin of the SIM800L module to digital pin 21 on the ESP32. <br>
•	Connect the GND pin of the SIM800L module to the GND on the ESP32. <br>
•	Connect the VCC pin of the SIM800L module to the 5V output on the ESP32. 
 
2.	Connect Fire Sensor: <br>
•	Connect the analog output pin of the fire sensor to analog pin 25 on the ESP32 (s1 in the code). <br>
•	Connect the digital output pin of the fire sensor to digital pin 18 on the ESP32 (E1 in the code). <br>
•	Connect Relay Module: <br>
•	Connect the input of the relay module to digital pin 18 on the ESP32 (E1 in the code). <br>
•	Connect the common (COM) terminal of the relay to one terminal of the fire alarm system. <br>
•	Connect the normally open (NO) terminal of the relay to the other terminal of the fire alarm system. 
 
3.	Power Supply: <br>
•	Power the Arduino using a USB cable connected to a computer or an external power supply. 
 
4.	Check Connections: 
•	Double-check all connections to ensure they are correctly made. <br>
•	Ensure that the SIM800L module is properly powered and has   a working SIM card inserted. 
 
5.	Upload the Code: <br>
•	Open the Arduino IDE, copy the provided code, and upload it to the Arduino board. <br>
•	Make sure the correct COM port and board are selected in the Arduino IDE. 
 
6.	Monitor Serial Output: <br>
•	Open the Serial Monitor in the Arduino IDE to monitor the output. <br>
•	The SIM800L module should respond with "OK" during initialization if the communication is established. 
 
7.	Cloud Setup: <br>
• Setup Arduino IOT cloud to monitor and and store the data. 
 
8.	Test the System: <br>
•	Introduce flame near the fire sensor to trigger an alert. <br>
•	Observe the Serial Monitor for messages indicating fire detection. <br>
•	Check whether the relay triggers and, if applicable, whether the SIM800L sends a message or makes a call based on the detected fire condition. 
   
9.	Adjust Threshold (if needed): <br>
• If false alarms or missed detections occur, adjust the threshold variable in the code to a suitable value. <br>
10.	Ensure Safety Precautions: <br>
• If testing involves real smoke or fire, exercise caution, and follow safety protocols. Perform tests in a controlled environment. 
</P>


