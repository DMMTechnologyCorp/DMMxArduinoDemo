# Arduino Control Demo with 3 Daisy-Chained DYN2 Servo Drives

This repository contains the code and instructions for an Arduino control demo using 3 daisy-chained DYN2 Servo drives. The demo demonstrates how to control multiple servo drives in a daisy-chain configuration using an Arduino microcontroller.

## Demo Video

Watch the demo video here: [Arduino Control Demo with DYN2 Servo Drives](https://www.youtube.com/watch?v=cxTCNnXewAU)

## Hardware Required

- Arduino board (e.g., Arduino Uno)
- 3 DYN2 Servo drives (In order to perfectly replecate the video. You can also run the code with only one drive!)
- Power supply for the servo drives
- Connecting cables (for power and communication)
- Breadboard and jumper wires (optional)

## Software Required

- Arduino IDE (latest version recommended)
- [DMM DRV Software](https://dmm-tech.com/Downloads.html) for drive configuration

## Getting Started

### 1. Download the Code

Go to the [releases page](https://github.com/DMMTechnologyCorp/DMMxArduinoDemo/releases/tag/V1.0) to download the latest release of the demo ino files.

### 2. Install the Arduino IDE

Download and install the latest version of the Arduino IDE from the [official website](https://www.arduino.cc/en/software).

### 3. Open the Arduino Project

Open the Arduino IDE and navigate to `File > Open...` to open the `DYN232M_Arduino_SampleCode_const_speed_demo.ino` or `DYN232M_Arduino_SampleCode.ino`  file you downloaded.

### 4. Connect the Hardware

1. **Connect the Arduino to the DYN2 Servo drives:**
   - Connect the TX pin of the Arduino to the RX pin of the first DYN2 Servo drive.
   - Connect the RX pin of the Arduino to the TX pin of the first DYN2 Servo drive.
   - Daisy-chain the remaining servo drives by connecting the TX pin of the first drive to the RX pin of the second drive, and so on.
   - Connect the GND pin of the Arduino to the GND pin of the first servo drive and daisy-chain the ground connections for all drives.
   - Connect the power supply to the servo drives as per the manufacturer's instructions.

2. **Connect the Arduino to your computer:**
   - Use a USB cable to connect the Arduino board to your computer.

### 5. Upload the Code

1. Select the appropriate board and port from the `Tools` menu in the Arduino IDE.
2. Click on the `Upload` button to upload the code to the Arduino.

### 6. Run the Demo

Once the code is uploaded, the Arduino will start sending commands to the DYN2 Servo drives, and you should see the servos moving according to the demo program.

## Customizing the Code

You can customize the demo by modifying the .ino file. The code is discussed in the video mentioned above to help you understand how to control the servo drives. Experiment with different movements and commands to see what you can achieve!

## Troubleshooting

- Ensure all connections are secure and correct.
- Verify that the power supply is sufficient for the servo drives.
- Check the Arduino serial monitor for any error messages or debugging information.

