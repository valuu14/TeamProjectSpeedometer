# TeamProjectSpeedometer

## Description

The project idea is to measure the speed of the user when moving towards an object in a straight line. Due to hardware constraints,there might be some issues regarding very close or very far measurements.

The sensor will measure the distance from its position to the first object met in a forward direction and continues to check it after short intervals of time. Once the distance starts to shrink, we assume the user started to move and we count that as a starting point. A few seconds (this constant will probably be configurable) after the distance input stops changing, we stop the timer. By subtracting the initial distance from the final one we get the travelled length, and dividing it by time measurements, we can compute the speed of the user. 

For the UI , we'll build an app where the user can see his current speed (this might not be extremely accurate and mostly depends on the sensor's capacity), the distance travelled, and the average speed.

## Pre-requisites

### Hardware

* Raspberry Pi Zero W ([details and specifications](https://itsfoss.com/raspberry-pi-zero-w/))
* Breadboard
* Male-to-female jumper wires
* HC-SR04+ distance sensor
