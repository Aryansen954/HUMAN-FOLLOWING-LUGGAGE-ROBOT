# HUMAN-FOLLOWING-LUGGAGE-ROBOT

This project is an **Arduino-based autonomous luggage bot** that follows a person using **IR sensors and an ultrasonic sensor**. The bot moves on 4 DC motors and intelligently navigates based on distance and obstacle sensing.

---

## 🔧 Features

- Follows a human using distance sensing (ultrasonic sensor)
- Detects direction using dual IR sensors
- Moves forward, stops, and turns left/right automatically
- Servo-based scanning motion for detection
- Uses motor driver shield to control 4 DC motors

---

## ⚙️ Hardware Used

- Arduino UNO
- L293D Motor Driver Shield
- 4 × DC Motors
- 1 × Ultrasonic Sensor (HC-SR04)
- 2 × IR Sensors
- 1 × Servo Motor (SG90)
- Power supply (battery)
- Chassis and wheels

---

## 🧠 Working Principle

- **Ultrasonic Sensor** detects the distance between the bot and the person.
- **IR Sensors** detect human presence/direction (left or right).
- **Servo Motor** sweeps the ultrasonic sensor to cover a wide area.
- The bot:
  - **Moves forward** when a person is in front (within 1–15 cm).
  - **Turns left/right** based on which IR sensor detects the human.
  - **Stops** if no one is in range (>15 cm).

---

## 📁 Code Overview

- Uses `AFMotor` library to control 4 motors.
- `NewPing` library for handling ultrasonic sensor.
- `Servo` library for controlling servo motor scan.
- Smart logic in `loop()` function checks sensor readings and makes movement decisions.

---

## 🛠️ Libraries Required

Install the following libraries from the Arduino Library Manager:
- `AFMotor`
- `NewPing`
- `Servo`

---

## 📷 Demo / Future Scope

Future enhancements:
- Use Bluetooth/GPS for path guidance
- Add voice commands or remote app control
- Implement weight sensing or theft alert system

---

## 🙋‍♂️ Author

**Aryan Sen**  
Electronics & Communication Engineering Student  
Feel free to connect on LinkedIn or GitHub!

---

## 📝 License

This project is open-source and available under the MIT License.
