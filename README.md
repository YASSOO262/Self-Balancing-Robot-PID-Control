# Self-Balancing-Robot-PID-Control
This project focuses on the design and control of a two-wheeled self-balancing robot based on the inverted pendulum principle. The robot maintains an upright position by continuously adjusting the wheel motion according to its tilt angle.

The project includes the mathematical modeling of the inverted pendulum, DC motor and wheel dynamics, followed by linearization of the system around the upright equilibrium point. The resulting equations are used to derive the system transfer function relating the motor input voltage to the robot's tilt angle.

A PID controller is then designed in MATLAB/Simulink to stabilize the robot and minimize the tilt-angle error. The controller is tested through simulation to evaluate the robot's stability, response time, and ability to recover from disturbances.

Main Objectives
Develop the mathematical model of a two-wheeled inverted pendulum.
Derive the transfer function of the system.
Design and tune a PID controller using MATLAB/Simulink.
Simulate the robot's balancing response.
Implement a proof-of-concept physical prototype.
Compare the simulated controller response with the prototype behavior.
Tools & Technologies
MATLAB
Simulink
PID Control
Mathematical Modeling
Inverted Pendulum Dynamics
DC Motor Modeling
Arduino
IMU/Gyroscope & Accelerometer
DC Motors and Motor Driver
**## Hardware Prototype

The physical prototype is a two-wheeled self-balancing robot designed based on the inverted pendulum concept.

The prototype consists of:

* **Two DC geared motors** to drive the left and right wheels.
* **Wheels and mechanical chassis** to support the robot and its electronic components.
* **Microcontroller** to process sensor measurements and execute the PID control algorithm.
* **IMU sensor** to measure the robot's tilt and angular motion.
* **Motor driver** to control the speed and direction of both motors.
* **Battery pack** to provide power to the motors and electronic components.

The controller continuously measures the robot's tilt angle and adjusts the motor speeds to keep the robot in an upright position.

### Prototype

![Self-Balancing Robot Hardware](hardware_prototype.jpg)

**Control flow:**

`IMU Sensor → Microcontroller → PID Controller → Motor Driver → DC Motors → Robot Motion → IMU Sensor`

This creates a closed-loop control system that continuously corrects the robot's position and maintains its balance.
**
