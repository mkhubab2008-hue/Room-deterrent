# Room deterrent 
<img width="396" height="448" alt="WhatsApp Image 2026-08-07 at 3 45 29 PM" src="https://github.com/user-attachments/assets/a341edb8-90a9-4b07-95a2-b362c55ba3e7" />

## Demo
Watch the room detterent in action
https://www.youtube.com/shorts/87MDrTLFvm4 

## About the Project
I wanted to use an ultra sonic sensor and an active buzzer, to sound an alarm everytime someone entered my room

## Hardware
This project consists of:
!) Arduino Uno
2) Solderless Breadboard
3) Active buzzer
4) hc-sr04 ultrasonic sensor module
5) Some jumper wires
6) USB A to B cable 
### Bill of Materials (BOM)

| Component | Quantity | Exact Price (USD) | Purchase Link |
| :--- | :---: | :---: | :--- |
| ELEGOO UNO R3 Board (Arduino-Compatible) | 1 | $14.99 | [Amazon Listing](https://www.amazon.com/dp/B008GRTSV6) |
| HC-SR04 Ultrasonic Distance Sensor | 1 | $3.95 | [Adafruit Listing](https://www.adafruit.com/product/3942) |
| 5V Active Piezo Buzzer | 1 | $1.95 | [Adafruit Listing](https://www.adafruit.com/product/1536) |
| Solderless Breadboard (830 Tie-Point) | 1 | $4.95 | [Adafruit Listing](https://www.adafruit.com/product/64) |
| Male-to-Male Jumper Wires (40-pack) | 1 | $3.95 | [Adafruit Listing](https://www.adafruit.com/product/758) |
| **Total Project Cost** | **—** | **$29.79** | — |

### Wiring Pinout Schedule

| Source Component | Source Pin | Target Component | Target Pin / Rail | Note |
| :--- | :--- | :--- | :--- | :--- |
| Arduino Uno | 5V | Breadboard | Positive Rail (+) | Main 5V power supply |
| Arduino Uno | GND | Breadboard | Negative Rail (-) | Common ground |
| HC-SR04 Sensor | VCC | Breadboard | Positive Rail (+) | 5V sensor power |
| HC-SR04 Sensor | GND | Breadboard | Negative Rail (-) | Sensor ground |
| HC-SR04 Sensor | Trig | Arduino Uno | Digital Pin 12 (D12) | Trigger signal input |
| HC-SR04 Sensor | Echo | Arduino Uno | Digital Pin 10 (D10) | Echo signal output |
| Piezo Buzzer | Anode (+) | Arduino Uno | Digital Pin 8 (D8) | Buzzer signal line |
| Piezo Buzzer | Cathode (-) | Breadboard | Negative Rail (-) | Buzzer ground |

##Overview 
This arduino based project uses an uno as the brain of this project where all the code is uploaded, a HC-SR04 Ultrasonic Sensor Module programmed to send a high signal back to the arduino when an objects comes with in 30 centimeters of it, a buzzer to sound an alarm, a solderless breadboard to connect and power all the sensors with the arduino, jumper wires for the connections and a usb cable to power and program the arduino with my pc.

##Wiring
I connected the arduinos 5v and GND pin to the breadboards positive and negative rail respectively, then I connected those positive and negative rails to the HC-SR04 Ultrasonic Sensor Module's VCC and GND respectively, I connceted the cathode and anode of the buzzer to the D8 pin on the arduino and the negative rail of the breadboard respectively, furthermore I connected the trig and echo pin of the HC-SR04 Ultrasonic Sensor Module to D12 and D10 on the arduino respectively
<img width="1600" height="1444" alt="WhatsApp Image 2026-08-07 at 4 20 36 PM" src="https://github.com/user-attachments/assets/52c26a63-9eb8-45fc-a0d8-9e632eaf8348" />

##Instructions 
Step-by-step Hardware Setup1.Power Down the Microcontroller:Disconnect your Arduino Uno from your computer and remove any external power adapters. Wiring components while the board receives current can cause short circuits or component damage.2.Establish Breadboard Power Rails:Insert one jumper wire from the 5V pin on the Arduino into the positive rail of your breadboard. Then, run a second jumper wire from any GND pin on the Arduino into the negative ground rail of the breadboard. This creates your shared power and ground buses.3.Mount the Ultrasonic Sensor. 4.Wire Sensor Power and Ground:Connect a jumper wire from the VCC pin of the ultrasonic sensor to the red positive power rail on your breadboard. Connect a jumper wire from the GND pin of the sensor directly to the blue negative ground rail.5.Connect Sensor Signal Lines:Plug a jumper wire into the terminal row connected to the sensor's Trig pin and run it directly to Digital Pin 12 on your Arduino. Connect another jumper wire from the Echo pin row on your breadboard directly to Digital Pin 10 on your Arduino.6.Mount and Wire the active Buzzer:Insert the buzzer into two separate rows on your breadboard. Identify the long leg (anode, positive terminal) and short leg (cathode, negative terminal). Run a jumper wire from the positive leg to Digital Pin 8 on your Arduino. Connect the negative leg to the blue negative ground rail on your breadboard.7.Verify and Upload:Double-check all connections against your code pin definitions (Trig on Pin 12, Echo on Pin 10, Buzzer on Pin 8). Once verified, plug the USB cable back into your computer and upload your code to test the alarm threshold.


## Reflections
This project tuaght me alot
1 How to use `if` and `else if` statements.
2 How to incorporate variables into my task
3 How to perform basic arithmetic operations in C++.
4 How to create conditions to make my hardwrare react to changes in rhe environment 
5 How to structure a simple command-line application.

Overall, it was a fun (and often frustrating) journey. The next I plan to make something even less useless and more complex :) .
