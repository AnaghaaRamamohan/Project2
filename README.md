# Project2
COMPETENT LIGHTING SYSTEM BASED ON MOTION DETECTION
The proposed system design is divided into three main components:
1.Arduino Microcontroller Circuit: Controls the entire system.
2.Ultrasonic Sensor: Detects the presence of a human or object within a specified distance in centimeters.
3.Relay Module: Facilitates automatic switching of the light.

# System Description
1.Functioning:
The operation of this project is straightforward and explained as follows:
When there is no human movement, the ultrasonic sensor does not detect any individual, and its OUT pin remains LOW.
2.Detection:
When an individual enters the room, the sensor detects the presence through ultrasonic waves if the distance is less than 30cm (predefined threshold).
Consequently, the output of the ultrasonic sensor goes HIGH.
3.Arduino Trigger:
The Data OUT of the ultrasonic sensor is connected to Digital Pin 8 of the Arduino.
When the sensor output is HIGH, the Arduino triggers the relay by setting the relay pin LOW (since the relay module is active LOW), turning the light ON.
4.Light ON:
The light remains ON as long as there is movement within the sensor's range.
5.No Movement:
When the person leaves the room, the distance between the sensor and the object exceeds 30cm.
The Data OUT of the ultrasonic sensor goes LOW, causing the Arduino to turn OFF the relay (setting the relay pin HIGH), thereby turning the light OFF.
6.Serial Monitor:
The distance between the ultrasonic sensor and the object is displayed on the serial monitor, along with variations in the distances.

# Implementation

-The circuit was successfully assembled, and the program was uploaded to the Arduino microcontroller chip.
-The ultrasonic sensor transmitted ultrasonic sound waves to detect the approaching object.
-The sensor was set to trigger at distances less than 30cm.
