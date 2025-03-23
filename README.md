# Gesture-Controlled-Robot
1. Connection of MPU6050 with ESP32
Connected an MPU6050 to an ESP32 as the following connection. The MPU6050 is an inertial measurement unit(IMU) that is a combination of gyroscope and accelerometer in all 6 dimension, which can detect the orientation, motion, and acceleration of the hand and give its value of each change to ESP32.
![image](https://github.com/user-attachments/assets/c782366c-1dca-45c8-a4c4-58504fc17494)
2. Simulation result of MPU6050
MPU6050 track each movement and send its value to ESP32 as shown in the result shown below.
![image](https://github.com/user-attachments/assets/9ec33a82-6c3b-4f12-b9a4-49ca29ba2543)
3. Speed Control with PWM Pins
Purpose : To control the speed of the motors driving the Mecanum wheels, we employed Pulse Width Modulation (PWM). This technique allows us to simulate varying levels of voltage by rapidly switching a digital signal between high (on) and low (off) states.

How PWM Pins Works :

The PWM signals are sent to the L298N motor driver through its enable pins (ENA and ENB). By adjusting these signals, we can finely control the speed of each motor based on user gestures.
Procedure :

Used the ESP32 PWM pins to generate Pulse Width Modulation (PWM) signals for the L298N motor driver.
Maped gesture intensities to speed levels (e.g., tilt angle to PWM duty cycle).
Ensure smooth acceleration and deceleration by fine-tuning the PWM signals.
Outcome : Enables precise control of motor speeds, ensuring the robot moves efficiently and responsively.
4. Wireless Data Transfer using WiFi (ESP-NOW Protocol)
Procedure:

Used ESP32 modules for both transmitting and receiving data.
Implemented the ESP-NOW protocol, which allows peer-to-peer communication with low latency.
Transmited gesture data from the glove as control commands (e.g., direction, speed).
![image](https://github.com/user-attachments/assets/d4848a37-aed7-4389-816f-71583d73b92f)

