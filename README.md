# Obstacle Avoiding Robot (2WD Smart Car)

This repository contains the hardware schematic and code for an autonomous 2WD (two-wheel drive) smart car built with an Arduino Uno. The robot uses an ultrasonic sensor to detect obstacles in its path and automatically changes direction to avoid collisions.

## 🚀 Features
* **Autonomous Navigation:** Continuously scans the environment and drives forward when the path is clear.
* **Obstacle Detection:** Uses ultrasonic sound waves to measure the distance to objects in real-time.
* **Dual Motor Control:** Independently drives the left and right wheels for precise steering and reversing using an L293D motor driver.

## 🛠️ Components Used
* 1x Arduino Uno
* 1x L293D Motor Driver IC
* 1x HC-SR04 Ultrasonic Sensor
* 2x DC Motors (Wheels)
* 1x 9V Battery (External power for the motors)
* 1x Breadboard & Jumper wires

## ⚡ Circuit Wiring
**Power Distribution:**
* The **9V Battery** powers the motors through the L293D driver IC to prevent overloading the Arduino.
* The **Arduino 5V** pin powers the HC-SR04 sensor and the logic pins of the L293D.
* All components share a **Common Ground (GND)**.

**Sensor & Motor Connections:**
* **HC-SR04:** Trigger and Echo pins are connected to the Arduino digital pins.
* **L293D:** 
  * Left pins control Motor 1 (Input logic connected to Arduino digital pins).
  * Right pins control Motor 2 (Input logic connected to Arduino digital pins).

## 💻 Code Setup
Upload the main `.ino` file to your Arduino Uno. Ensure that the pin definitions in the code match your physical wiring for the ultrasonic sensor (Trig/Echo) and the L293D driver inputs.

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
