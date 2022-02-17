# Libraries and the Semester Project

You are allowed to use _some_ Wired (Arduino) libraries in the semester project. 

## Libraries Usage

Arduino library usage by component:

| Component      | Library Ok for Project? | 
| -------------- | ----------------------- |
| DC Motor       | No                      |
| Servo Motor    | Yes                     |
| DHT11          | Yes                     |
| LCD            | Yes                     |
| Water Sensor   | No                      |
| DS 1307 RTC    | Yes                     |
| Potentiometers | No                      |
| Thermister     | No                      |


## The Wired Library
- GPIO
	- `pinMode` may NOT be used. Pins must be configured and read/written using registers as used in the labs
	- `digitalRead` and `digitalWrite` may NOT be used
- ADC
	- `analogRead` and `analogWrite` may NOT be used. You can look at the method source if you are unsure what steps need to be taken to read or write.
- You *may* use the `Serial` library methods
- Timer configurations must be performed as they were in class

## Possible Issues
Depending on your design, you may run into conflicts between devices when using interrupts. If this happens, contact your TA or Dr. Lancaster to discuss.
