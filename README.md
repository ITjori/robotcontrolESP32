# Task 3

**(Robot control using ESP32)**

This approach enables real-time control of the robot using a mobile application.

## **Steps to Control ESP32 via MIT App Inventor**

***1.   Connect ESP32 to WiFi (Client or AP Mode):***
 
	•	Client Mode: Connect ESP32 to a local WiFi network using SSID and password, allowing communication with other devices on the same network.
	•	AP Mode: Configure ESP32 to create its own WiFi network, enabling direct connection from a phone.
 
***2.	Setup the Server on ESP32:***
 
	•	In the ESP32 code, set up a WebServer to handle HTTP requests. Define endpoints like /direction to receive control commands (e.g., forward, left, stop).
 
***3.	Configure MIT App Inventor:***
 
	•	Use MIT App Inventor to design a mobile interface with buttons for control. Add a Web Component to send HTTP requests (GET method) to the ESP32 IP address.
	•	Each button triggers a specific URL request
 
***4.	Connect Mobile Device to WiFi:***
 
	•	Ensure the mobile device is connected to the same WiFi network as the ESP32 (Client Mode) or directly to ESP32’s WiFi (AP Mode).
 
***5.	Send Commands and Monitor Output:***
 
	•	When a button is pressed, MIT App Inventor sends the corresponding HTTP request to ESP32.
	•	ESP32 processes the command and responds by performing the appropriate action (e.g., forward).
	•	Output is visible on the Serial Monitor
