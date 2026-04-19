Sonar Based Object Detector

About the Project

This project is a simple sonar-based object detection system built using an ultrasonic sensor and a servo motor.
The idea is to make something similar to a basic radar.
The ultrasonic sensor is mounted on a servo motor, and it rotates from 0° to 180°, checking for objects in front of it.
At each angle, it measures the distance and sends the data to the Arduino.

Components Used

- Arduino board
- Ultrasonic sensor (HC-SR04)
- Servo motor
- Jumper wires
- Breadboard

How it Works

The working is pretty straightforward:
- The servo motor rotates slowly from 0° to 180°
- At every position, the ultrasonic sensor sends a signal
- It calculates how far an object is based on the echo
- The Arduino prints the angle and distance
This keeps repeating, so it continuously scans the area.

Output

You can see the output in the Serial Monitor, where it shows:
- Angle
- Distance
I have also connected it to tools like Processing for a radar-style display.

Connections

Ultrasonic Sensor
- VCC → 5V
- GND → GND
- Trig → Digital Pin
- Echo → Digital Pin

Servo Motor
- VCC → 5V
- GND → GND
- Signal → PWM Pin

How to Run

1. Connect all the components properly
2. Upload the code to Arduino
3. Upload code in Processing software also
4. Open Serial Monitor
5. You should start seeing distance values as the sensor rotates

What I Learned

- How ultrasonic sensors work
- How to control a servo motor
- Reading and using sensor data
- Basic hardware + software integration


Future Improvements

- Add a proper radar visualization
- Improve accuracy
- Make it faster and smoother
