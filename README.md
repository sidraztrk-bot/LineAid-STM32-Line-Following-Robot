# LineAid – STM32 Line Following Robot

LineAid is an STM32-based autonomous line-following robot developed as a university embedded systems project.

The project was inspired by autonomous medicine delivery systems in hospitals and healthcare facilities. The implemented prototype focuses on reliable line tracking, path correction, and route navigation using infrared sensors.

---

## Project Overview

The robot follows a black line on a white surface using five infrared sensors connected to an STM32 microcontroller.

Based on sensor readings, the robot can:

* Follow a predefined path
* Detect left turns
* Detect right turns
* Detect start and finish points
* Recover from temporary line loss
* Adjust motor movement in real time

The project serves as a prototype for future autonomous indoor delivery systems.

---

## Mechanical Design

The robot chassis was designed using **Rhino 3D**.

The structure was manufactured using **laser-cut MDF wood panels**, then assembled to create a lightweight mobile platform capable of carrying small payloads.

Unlike many educational line-following robots that use ready-made chassis kits, the mechanical structure of LineAid was custom-designed and fabricated specifically for this project.

---

## Hardware Components

* STM32F103 Blue Pill
* 5× IR Line Tracking Sensors
* L298N Motor Driver
* 2× DC Motors
* Battery Pack
* Laser-Cut MDF Chassis

---

## Software Features

### Line Following

The robot continuously reads five infrared sensors and determines its position relative to the line.

### Path Correction

When the line is temporarily lost, the robot uses the last detected direction to recover the path.

### Turn Detection

Different sensor combinations are used to identify:

* Left turns
* Right turns
* Junction transitions

### Start / Finish Detection

Special sensor patterns are used to identify the beginning and end of the route.

### PWM Motor Control

Motor speed is controlled using STM32 timers and PWM signals.

Used peripherals:

* TIM2 PWM
* TIM3 PWM
* GPIO Inputs
* GPIO Outputs

---

## Development Tools

* STM32CubeIDE
* STM32 HAL Library
* Rhino 3D
* Laser Cutter

---

## Future Improvements

Potential future developments include:

* Autonomous medicine delivery
* Hospital corridor navigation
* Stop-and-wait stations
* Multi-destination routing
* Obstacle avoidance

---

## Author

Sıdra ÖZTÜRK

Biomedical Engineering Student
