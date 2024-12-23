2014-Aerial-Assist-FRC-FIRST-Robotics-Power-Electronics

![image](https://github.com/user-attachments/assets/10e91864-fe47-48b0-8009-543a6d67d577)


This repository contains documentation and resources related to the power electronics setup for the 2014 FIRST Robotics Competition (FRC) robot built during my high school senior year. The focus of the project was on wiring a Power Distribution Panel (PDP) and integrating DC motors, relays, and solenoids to control the robot’s movements and actuators.



The project involved the design and implementation of the electrical system that powers and controls the robot’s motors and actuators, ensuring smooth and reliable operation during the Aerial Assist challenge.



Overview



In the 2014 FRC season, the robot needed to be equipped with a power system capable of handling various motors, sensors, and actuators while providing sufficient current and voltage for all components. This was achieved by setting up and wiring the Power Distribution Panel (PDP) and integrating it with motors, relays, and solenoids for optimal performance.



Key Components

• Power Distribution Panel (PDP): The central hub that distributes power to the robot’s electrical components.

• DC Motors: Used to drive the robot’s wheels and various actuators.

• Relays: Employed to control high-power components like motors and solenoids.

• Solenoids: Used for controlling pneumatic actuators, such as a claw or other manipulative components.



Goals of the Project

• Properly wire and configure the PDP to handle multiple motor controllers and actuators.

• Implement control systems for DC motors, relays, and solenoids to ensure reliable robot operation.

• Work with various sensors and feedback systems for efficient power usage.



Features

• Power Distribution Panel Setup: Wiring and configuring the PDP to distribute power safely and effectively to all robot components.

• Motor Control: Wiring and interfacing with DC motors to drive wheels, wheels with encoders, and other moving parts.

• Relay Control: Setup of relays for switching high-current devices on and off.

• Solenoid Control: Integration of solenoids to control pneumatic actuators, which are key in various FRC mechanisms (e.g., claw openings and ball manipulations).

• Safety Protocols: Adhering to safety regulations by wiring breakers and fuses to ensure components don’t overheat or become damaged.



Installation & Setup



Prerequisites



Before you begin, ensure you have the following:

1. FRC Electrical Components:

• Power Distribution Panel (PDP)

• Motor Controllers (e.g., Talon SRX, Victor SP, etc.)

• DC Motors (12V)

• Relays (e.g., Spike Relay)

• Solenoids

• Wires, Breakers, and Fuses

2. FRC Robot Software (for control systems):

• Install LabVIEW or C++ development environments to program the control system (if you are handling the software side as well).

• Ensure proper wiring of the robot’s CAN bus or PWM (Pulse Width Modulation) connections for controlling motors.



Wiring Diagram



Below is a simplified representation of how the Power Distribution Panel (PDP) is wired in this setup:

1. Power Distribution Panel (PDP):

• The PDP is the central hub that receives power from the battery and sends it to various components.

• The PDP has multiple outputs (e.g., 12V and 5V) that supply power to motors, relays, and solenoids.

• Example Wiring:

• 12V from the PDP is routed to motor controllers for DC motors.

• A relay is wired to switch on/off high-power components like the compressor or pneumatic solenoids.

• Solenoids are connected to the PDP via the PWM ports or through digital outputs that control the solenoids.

2. DC Motor Wiring:

• Motors like CIM motors or Mini CIM motors are connected to motor controllers, which in turn are powered by the PDP.

• Motor controllers are wired to provide forward/reverse control for the motors, and encoders may be used for feedback.

3. Relay Wiring:

• Relays are used to control high-current systems like solenoids and actuators. They provide an on/off signal.

• Each relay is connected to the PDP and controlled via the robot’s control system.

4. Solenoid Wiring:

• Pneumatic solenoids are powered through the PDP. The control signal to the solenoid is typically managed by the robot’s Digital I/O or Relay channels.



Example Wiring Setup



Wiring the Power Distribution Panel (PDP)



Battery (+)  -------------------------> PDP (12V Input)

Battery (-)  -------------------------> PDP (Ground)

 

Outputs:

1. PDP 12V Output -----------------> Motor Controller 1 (Motor 1)

2. PDP 12V Output -----------------> Motor Controller 2 (Motor 2)

3. PDP 12V Output -----------------> Relay (for solenoids or other actuators)

4. PDP 5V Output -----------------> Sensors (e.g., encoder, sensors)



Wiring a DC Motor to a Motor Controller



PDP 12V Output  -----------------> Motor Controller  (e.g., Talon SRX)

Motor Controller (PWM) ----------> Motor (DC Motor)

Motor Controller (CAN) ---------> PDP (via CAN bus)



Wiring a Solenoid to a Relay



PDP 12V Output -----------------> Relay (e.g., Spike Relay)

Relay (PWM) ---------------------> Solenoid

Relay (Control) -----------------> Control Signal (from robot’s control system)



License



This project is licensed under the MIT License - see the LICENSE file for details.



Contributing



If you’d like to contribute to this project or suggest improvements, feel free to fork the repository and submit pull requests. Please ensure that your changes are well-documented and tested.



Acknowledgments

• Thanks to FIRST Robotics for providing the framework and components necessary to build the robot.

• Special thanks to the mentors, teammates, and the broader FRC community for their support and guidance during this project.

MIT License
