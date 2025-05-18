# Robotics-Project
Wirelessly Controlled Differential Drive Robot using ROS2

Intro:

A wirelessly controlled differential drive robot using ROS2 involves creating a robot that can move by independently controlling two wheels on either side. ROS2 (Robot Operating System 2) serves as the middleware to manage robot communication, control algorithms, and sensor integration. The wireless control is typically achieved using Wi-Fi or Bluetooth, allowing remote operation via a computer, smartphone, or joystick. This setup is common in robotics research and applications where mobility and remote operation are essential.

List of components:

Two 12V N20 Dc motors 300 rpm
L298N motor driver
Raspberry Pi 3b+
Castor wheel
Two wheels 44mm diameter
12V battery for motor driver to motors
20000 mah power bank for Raspberry Pi
Breadboard ground rail for common ground
Fiber platform for bot

Working:

<img src="Diff Drive Robot.jpg">
This is the build of the bot.
A code has been written in the rpi interface which can control the bot. There are 2 ROS nodes here, one for teleopkey and one for motor control. The rpi is being controlled by remote SSH. We can use designated keys on the laptop to control the bot. The rpi receives the instructions first and sends relevant info to the motor driver which sends the signals to the motors in order to control the movement of the bot. The keys for moving are w, a, s, d for front, left, back, right respectively. Long pressing a key results in the bot moving in that direction. Spacebar to stop the bot and get it to a standstill.

Conclusion:

The wirelessly controlled differential drive robot using ROS2 demonstrates the effective integration of hardware and software to achieve remote mobility. Utilizing ROS2 for communication and control, the robot can be operated seamlessly via a laptop using SSH. The use of two ROS nodes, one for teleoperation and the other for motor control, ensures a modular and efficient design. The system's ability to interpret key inputs and control the motor driver through the Raspberry Pi highlights the practicality of using ROS2 in robotic applications. This project serves as a robust foundation for future improvements, such as adding autonomous navigation or incorporating sensor feedback.
