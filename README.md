# River Cleaner Robot

## Overview
This project implements an autonomous river cleaning robot using Arduino and ultrasonic sensors. The robot is designed to navigate along the river, avoid obstacles, and continuously collect waste using a conveyor belt. It utilizes ultrasonic sensors for edge detection and obstacle avoidance, and it displays real-time status updates on an LCD.

---

## Features
- **Obstacle Avoidance**: Detects obstacles in front using an ultrasonic sensor and takes appropriate action.
- **Edge Detection**: Uses ultrasonic sensors on the left and right to detect edges and avoid falling.
- **Waste Collection**: A conveyor belt is continuously running to collect waste from the water surface.
- **LCD Display**: Provides real-time updates about distances, actions, and the robot's status.
- **Buzzer Alerts**: Alerts when obstacles or edges are detected.

---

## Components Used

### Hardware
1. **Arduino Uno**
2. **Ultrasonic Sensors (3)**
   - Front: Obstacle detection
   - Left and Right: Edge detection
3. **Motor Driver (L298N)**
   - Controls wheel motors and conveyor belt motors
4. **DC Motors (4)**
   - Two for wheels
   - Two for the conveyor belt
5. **LCD Display (16x4, I2C)**
6. **Buzzer**
7. **Power Supply**
   - Arduino powered via USB
   - Motors powered via battery pack (7.4V)

### Software
- **Arduino IDE**: For writing and uploading code to the Arduino Uno.

---

## Pin Configuration

### Arduino Pin Assignments
#### Motors (Wheels):
- **IN1**: Pin 9
- **IN2**: Pin 8
- **IN3**: Pin 11
- **IN4**: Pin 10

#### Motors (Conveyor):
- **IN1**: Pin 4
- **IN2**: Pin 5
- **IN3**: Pin 6
- **IN4**: Pin 7

#### Ultrasonic Sensors:
- **Front Sensor**:
  - TRIG: A0
  - ECHO: A1
- **Left Sensor**:
  - TRIG: A2
  - ECHO: A3
- **Right Sensor**:
  - TRIG: Pin 2
  - ECHO: Pin 3

#### Other Components:
- **Buzzer**: Pin 13
- **LCD (I2C)**:
  - SDA: A4
  - SCL: A5

---

## Code Explanation
The code has the following main functionalities:
1. **Ultrasonic Distance Measurement**: Measures distances from the front, left, and right sensors.
2. **Motor Control**: Controls the wheel and conveyor motors based on sensor input.
3. **Obstacle Avoidance**: Stops the robot and alerts when obstacles are detected in front.
4. **Edge Detection**: Turns the robot in the opposite direction when edges are detected.
5. **LCD Updates**: Continuously displays sensor readings and actions on the LCD.
6. **Conveyor Activation**: Keeps the conveyor belt running continuously to collect waste.

---

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/river-cleaner-robot.git
   ```
2. Open the `ultrasonic_edge_navigation.ino` file in Arduino IDE.
3. Connect your Arduino Uno to your PC.
4. Verify and upload the code to the Arduino board.
5. Assemble the hardware as per the wiring diagram.
6. Power the robot and observe its functionality.

---

## Testing and Debugging
- Use the Serial Monitor (set to 9600 baud) to debug sensor readings and actions.
- Ensure all connections are secure and components are powered correctly.
- Simulate edges and obstacles for testing before running in real-world conditions.

---

## Future Enhancements
- Integrate a camera module for object detection and advanced waste identification.
- Add IoT features to monitor robot activity remotely.
- Improve energy efficiency with solar-powered batteries.

---

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your enhancements.

---

## Contact
For any queries or suggestions, feel free to contact:
- **Name**: Ravindu Sahan
- **Email**: ravinduvinushasahan@gmail.com
- **GitHub**: [Your GitHub Profile](https://github.com/Ravindu-VS)

