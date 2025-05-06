# RC_Rover
Setup Overview
Arduino Uno:
  1.Motor Control: The Uno will handle the PWM signal for the ESC to control the DC motor's speed.
  2.Servo Control: The Uno will also manage the PWM signal for the servo motor to control steering.
  3.Power: The ESC can power the Uno through the VIN pin.
  
ESP32:
  1.Bluetooth Communication: The ESP32 will manage Bluetooth communication with your controller.
  2.Serial Communication: The ESP32 will send commands to the Uno via serial communication.
  
Communication:
  1.The ESP32 will send commands (e.g., speed, direction, steering angle) to the Uno via serial communication.
  2.The Uno will receive these commands and control the motor and servo accordingly.
  
Code:
  Arduino Uno Code:
    Receive serial commands from the ESP32.
    Control the ESC (speed and direction).
    Control the servo motor (steering).
    
  ESP32 Code:
    Set up Bluetooth communication.
    Receive commands from the Bluetooth controller.
    Send commands to the Uno via serial.
