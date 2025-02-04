# 🚨Landslide Detection System with SMS and Call Alert

Welcome to the **Landslide Detection System** repository! This project uses ultrasonic sensors and a SIM800L GSM module to detect potential landslides and send alerts via SMS and phone calls.🚧📱

---

## 🛠️ **Features**

- **Dual Ultrasonic Sensors**: Monitors distances using two sensors for enhanced accuracy.
- **SMS Alerts**: Sends an SMS when a potential landslide is detected.
- **Call Alerts**: Initiates a phone call to a predefined number during emergencies.
- **Arduino Compatible**: Built using Arduino IDE and compatible libraries.

---

## 🧩 **Hardware Requirements**

- Arduino Uno (or compatible board)
- SIM800L GSM module
- Ultrasonic Sensors (2 units)
- Breadboard and jumper wires
- Power supply

---

## 📜 **How It Works**

1. The system uses two ultrasonic sensors to measure distances.
2. If the sum of distances detected falls within the critical range (150-300 cm):
   - An SMS is sent to the specified phone number.
   - A call is initiated to alert the user.
3. The system continuously monitors and updates distances in real-time.

---

## 🚀 **Setup and Installation**

1. **Connect the Components**:
   - Connect the ultrasonic sensors to analog pins A0, A1, A2, and A3.
   - Connect the SIM800L module to digital pins 10 (RX) and 11 (TX).

2. **Upload the Code**:
   - Open the provided `.ino` file in the Arduino IDE.
   - Replace `+91XXXXXX` with your phone number in the code.
   - Upload the code to your Arduino board.

3. **Power Up**:
   - Ensure the SIM800L module is powered by a stable 5V source.
   - Turn on the system and monitor the serial output for status updates.

---

## 📝 **Code Explanation**

- **`SonarSensor()`**:
  Measures the distance using the ultrasonic sensor.
- **`SendMessage()`**:
  Sends an SMS alert to the specified number.
- **`callNumber()`**:
  Initiates a phone call to the predefined contact.
- **`RecieveMessage()`**:
  Handles incoming SMS functionality (optional feature).

---

## 📊 **Sensor Configuration**

| **Sensor**   | **Trigger Pin** | **Echo Pin** |
|--------------|-----------------|--------------|
| Sensor 1     | A0              | A1           |
| Sensor 2     | A2              | A3           |

---

## ⚠️ **Important Notes**

- Ensure your SIM card has sufficient balance for SMS and calls.
- Check the SIM800L's network connectivity before use.
- Use a stable power source for the SIM800L to prevent unexpected behavior.

---

## 🎉 **Contributing**

Contributions are welcome! Feel free to submit a pull request or open an issue to improve this project. 🌟

---

**Enjoy building and stay safe! 🚀**

